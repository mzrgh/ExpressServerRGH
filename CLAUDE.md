# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

- `npm start` - Start the development server using nodemon (auto-reloads on changes)
- `npm test` - Run tests (currently not configured)

## Project Architecture

This is a simple Express.js personal website project with the following structure:

### Core Files
- `app.js` - Main Express server file that serves static files and handles the root route
- `index.html` - Personal website homepage in Spanish for Raúl González
- `styles.css` - Stylesheet with modern design using flexbox and clean typography
- `package.json` - Node.js project configuration with Express and nodemon dependencies

### Server Configuration
- Port: 3000
- Static file serving enabled for the entire root directory
- Single route handler for "/" that serves index.html
- Uses nodemon for development hot-reloading

### Frontend Structure
The website is a single-page personal portfolio with:
- Header with name and description
- Navigation menu (Inicio, Sobre mí, Proyectos)
- Three main sections: welcome, about me, and projects
- Project links reference future subdirectories (proyecto1/, proyecto2/)
- Modern CSS styling with dark blue theme (#2c3e50, #34495e)

### Dependencies
- `express ^5.1.0` - Web framework
- `nodemon ^3.1.10` - Development dependency for auto-restarting server

The project is set up as a foundation for hosting multiple sub-projects accessible through the main landing page.