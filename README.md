# WordPress Persistence Lab

## Objective
Demonstrate the difference between ephemeral containers and persistent storage in Docker.

## Scenario
During testing, uploaded images disappeared after container recreation.

## Investigation
- Network connectivity tested using a debug container
- Container lifecycle analyzed
- Data storage location identified

## Root Cause
WordPress uploads were stored inside the container filesystem.

## Solution
Implemented Docker named volumes to persist application data.

## Stack
- Docker Compose
- WordPress
- MySQL 8.4

## Learning Outcomes
- Stateful vs Stateless containers
- Docker volumes
- Troubleshooting methodology
