# AEROSAR

## AI-Enabled Autonomous Emergency Search and Rescue Drone

AEROSAR is a team project combining simulation, ROS 2, AI perception, navigation, backend services, and a live monitoring dashboard.

## System Flow

Webots / Sensors → ROS 2 → AI Perception → Navigation → Backend → WebSocket → Dashboard

## Repository Structure

- worlds/ — simulation worlds
- drone_description/ — drone model and description
- aerosar_msgs/ — custom ROS 2 messages
- perception/ — AI detection and sensor fusion
- navigation/ — navigation and search logic
- backend/ — API, database, risk scoring and offline sync
- frontend/ — monitoring dashboard
- launch/ — system launch files
- scripts/ — integration, testing and demo scripts
- docs/ — documentation

## Branch Workflow

feature branches → develop → integration testing → main

### Feature Branches

- feature/webots
- feature/ai
- feature/navigation
- feature/backend
- feature/dashboard
- feature/integration

## Member 6 Responsibilities

Integration, testing, ROS 2 debugging, launch files, system testing, demo coordination, and GitHub workflow management.
