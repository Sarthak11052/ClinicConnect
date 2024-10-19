
# HealthCare Management System

The HealthCare Management System is a comprehensive solution designed to simplify patient registration, appointment scheduling, and medical appointment management. With full responsiveness and secure storage, it is built for modern healthcare needs, making it easier for both patients and administrators to manage appointments efficiently.

## Features

- **Patient Registration**: Users can register and manage their profiles.
- **Appointment Scheduling**: Patients can schedule appointments with healthcare providers.
- **Appointment Management**: Administrators can confirm, cancel, and reschedule appointments.
- **SMS Notifications**: Integrated with Twilio for appointment confirmations and reminders.
- **Secure File Storage**: Utilizes Appwrite for safe and secure file storage of patient data and medical records.
- **Responsive Design**: Fully responsive, ensuring optimal user experience across all devices.

## Tech Stack

- **Frontend**: Next.js with TypeScript, ShadCN for design components
- **Styling**: TailwindCSS
- **Notifications**: Twilio (for SMS notifications)
- **File Storage**: Appwrite
- **Hosting**: (add your hosting provider here)

## Installation

To set up the project locally:

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/healthcare-management.git
   ```

2. Navigate to the project directory:

   ```bash
   cd healthcare-management
   ```

3. Install the dependencies:

   ```bash
   npm install
   ```

4. Set up your environment variables by creating a `.env` file:

   ```
   NEXT_PUBLIC_TWILIO_ACCOUNT_SID=your_twilio_account_sid
   NEXT_PUBLIC_TWILIO_AUTH_TOKEN=your_twilio_auth_token
   NEXT_PUBLIC_APPWRITE_ENDPOINT=your_appwrite_endpoint
   NEXT_PUBLIC_APPWRITE_PROJECT_ID=your_appwrite_project_id
   ```

5. Start the development server:

   ```bash
   npm run dev
   ```

   The app will be accessible at `http://localhost:3000`.

## Key Features

- **Patient Registration**: 
  - `POST /api/patients/register`: Register a new patient.
  - `GET /api/patients/:id`: Retrieve patient details.

- **Appointment Management**: 
  - `POST /api/appointments`: Schedule a new appointment.
  - `PUT /api/appointments/:id/confirm`: Confirm an appointment.
  - `DELETE /api/appointments/:id/cancel`: Cancel an appointment.

- **SMS Notifications**: 
  - Automatically sends SMS notifications for appointment confirmations, reminders, and cancellations via Twilio.

