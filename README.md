# CV Personal Statements Game

## Business Problem

Many trainees write impersonal CV Personal Statements. We want a fun way to test how personal their statements are during class.

This project provides a website where:

- A volunteer can start a game.
- Trainees can join a started game.
- Each trainee enters their name and personal statement from their CV.
- The game shows one statement at a time (without the name) along with a list of trainees.
- Trainees guess whose statement it is.
- After everyone votes, the next statement is shown.
- At the end, the game shows how personal each statement was based on correct guesses.

## Requirements

- Simple frontend and a backend to coordinate state across users.
- No long-term persistence. All game data should be deleted after the game ends or after 24 hours.
- Access control: probably a password for joining a game, set by the volunteer.
- Must be functional, accessible, tested, and easy for CodeYourFuture volunteers to deploy and maintain.

## Features

- Real-time multiplayer game for a classroom setting.
- Trainees can enter and guess personal statements.
- Volunteer can control and start the game.
- Scoring system shows which statements were personal vs. generic.

## Solution
We built a full-stack multiplayer web application that transforms CV personal statement review into an interactive classroom game.

The solution allows a volunteer to create and manage a game session while trainees join using a shared game link and optional passcode. Each participant submits a personal statement anonymously, and the system presents statements one at a time for players to guess who wrote them.

The application coordinates game state in real time across multiple users using a FastAPI backend and polling-based frontend updates. At the end of the game, results and scores reveal how identifiable or generic each statement was, helping trainees improve the authenticity of their CV writing in a fun and engaging way.

The system was designed to be lightweight, accessible, and easy to deploy, using:

Frontend: Vanilla JavaScript + Vite
Backend: Python + FastAPI
Database: PostgreSQL + SQLAlchemy
Database migrations: Alembic
Hosting & automation: Coolify + Cron jobs for automatic cleanup of expired games

Additional features included:

Host controls for starting and ending games
Input validation and duplicate-player prevention
Passcode-protected game access
Automatic deletion of game data after 24 hours
Responsive and user-friendly interface for classroom use

## Tech Stack

- Frontend: HTML, JavaScript, Tailwind CSS
- Backend: Python,FastAPI
- Database: PostgreSQL
- Dev environment: Vite

## Video Demo

https://cv-statement-detective.hosting.codeyourfuture.io/

https://github.com/user-attachments/assets/8eea3567-f7f0-4c9f-b8bc-4da15b77534e


