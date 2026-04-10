# Smart Elevator Control System (ER Design)

## Overview

This system is designed to manage multiple elevators across multiple buildings, ensuring efficient ride allocation, real-time monitoring, maintenance tracking, and usage analytics.

## Objective

- Manage multiple buildings and their infrastructure
- Track elevators and their operational zones
- Handle floor-level ride requests
- Allocate elevators efficiently
- Monitor real-time elevator status
- Maintain maintenance history
- Store ride logs for analytics and optimization

## Entities

- buildings
- floors
- elevator_shafts
- elevators
- elevator_floor
- floor_requests
- ride_assignments
- ride_logs
- elevator_status_log
- maintenance_system

## Supported Queries ❓

- How many buildings are connected?
- How many elevators exist per building?
- Which floors belong to a building?
- Which elevators serve which floors?
- Which requests were generated from which floors?
- Which elevator handled a request?
- Which requests are pending?
- How many rides were completed today?
- Which elevator handled the most requests?
- What is the current status of elevators?
- Which elevators are under maintenance?

## Relationships

- One Building has many Floors
- One Building has many Elevators
- One Shaft contains one Elevator
- One Elevator serves many Floors
- One Floor can be served by many Elevators
- One Floor generates many Requests
- One Request is assigned to one Elevator
- One Elevator completes many Rides
- One Elevator has many Status Logs
- One Elevator has many Maintenance Records

### Feedback is most welcome 😊