# Gojek Ride Request Sequence Diagram Assignment

## Objective

The objective of this assignment is to create a sequence diagram that illustrates the flow of operations when a customer requests a ride using the Gojek mobile app. This exercise will help you understand the API flow and how different systems interact during the ride request process.

## Systems Involved (API Integration/System Integration)

For this assignment, we will focus on the following five systems that play a crucial role in the ride request process:

1. **Mobile App**: The user interface used by customers to request rides.
2. **Middleware**: This component manages communication between the mobile app and backend services, acting as an intermediary.
3. **Ride Management Service**: Responsible for processing ride requests, managing driver assignments, and updating ride statuses.
4. **Driver Management Service**: Handles driver registration, availability status, and all driver-related data.
5. **Payment Processing Service**: Manages all payment transactions securely, ensuring a seamless payment experience for users.

## Typical Flow for Requesting a Ride

The typical flow for requesting a ride through the Gojek app involves several steps:

1. **Customer signs in to the mobile app**: Users authenticate themselves to access ride services.
2. **Home screen displays available services**: The app presents options such as different ride types (e.g., GoRide) and estimated fares.
3. **Customer requests a ride**: The user selects their pickup location and destination, initiating the ride request.
4. **Request sent to Middleware**: The mobile app sends the ride request details to the middleware for processing.
5. **Middleware forwards request to Ride Management Service**: The middleware communicates with the Ride Management Service to identify available drivers.
6. **Ride Management Service checks Driver Management Service**: It retrieves information about available drivers based on their status and proximity to the pickup location.
7. **Driver assigned based on availability**: The Ride Management Service assigns an available driver to fulfill the customer’s request.
8. **Confirmation returned through Middleware**: The Ride Management Service sends confirmation details (including driver information) back through the middleware to the mobile app.

## Sequence Diagram Steps

Below are detailed steps for your sequence diagram:

1. **User clicks "Request Ride" in Mobile App**: This action triggers the entire ride request process.
2. **Mobile App sends request to Middleware**: The app transmits the user's ride request details, including pickup and drop-off locations.
3. **Middleware forwards request to Ride Management Service**: The middleware relays the request for further processing by the Ride Management Service.
4. **Ride Management Service queries Driver Management Service for available drivers**: It checks which drivers are available based on their status and proximity to the requested pickup location.
5. **Driver Management Service returns list of available drivers**: This service provides data on drivers who can accept the request at that moment.
6. **Ride Management Service assigns a driver**: A suitable driver is selected from the list of available drivers and assigned to fulfill the customer’s ride request.
7. **Ride Management Service sends confirmation back to Middleware**: Confirmation of driver assignment is sent back through the middleware, including essential details like driver name and vehicle information.
8. **Middleware returns confirmation to Mobile App**: The final confirmation is displayed in the mobile app, allowing users to see their assigned driver’s details.

## Assignment Instructions

1. Create a sequence diagram using any diagramming tool (e.g., Lucidchart, Draw.io, or Microsoft Visio).
2. Include all systems involved as lifelines in your diagram.
3. Use arrows to indicate the flow of messages between systems based on the steps outlined above.
4. Clearly label each interaction with brief descriptions that explain what each step entails.
5. Submit your completed sequence diagram along with a detailed explanation of each step in the flow.

### Submission Format

- File format: PDF or image (PNG/JPEG)
- Include your name and date on your submission.

## Conclusion

This assignment will enhance your understanding of how various systems interact within a real-world application like Gojek during a ride request process. You will gain insights into API integration and system communication dynamics, which are essential skills in software development and system design. Good luck with your work, and be creative with your diagram!
