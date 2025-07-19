## 🛠️ Feature List

### 🔐 User Authentication
- **Description**: Allow users to securely log in to the app using a username and password.
- **User Story**: As a user, I want to log into my account so I can securely access and manage my home data.
- **Acceptance Criteria**:
  - Users must verify their account credentials before access is granted.
  - Login form accepts username and password.
  - Incorrect credentials display a helpful error message.

---

### 🏠 Room-Based Item Lookup & Management
- **Description**: Users can manage and view items specific to each room of their home. The homepage will show a stylized blueprint of the house, and clicking on a room displays all associated data.
- **User Story**: As a homeowner, I want to click on a room in my house and view all relevant info for that space so I can stay organized and access it easily.
- **Stored Information per Item (e.g., appliances, paint, flooring)**:
  - Item type (e.g., appliance, wall paint, flooring)
  - Make, model, and serial number
  - Install date
  - Receipt (image or file)
  - Link to PDF of product manual
  - Servicer company (name and phone number)
  - Maintenance schedule
  - Maintenance records:
    - Date of service
    - Company
    - Service person
    - Rating
    - Receipt

---

### 🔔 Maintenance Reminders
- **Description**: The system will send timely reminders to the user for upcoming or overdue maintenance tasks based on their maintenance schedules.
- **User Story**: As a user, I want to receive reminders for maintenance so I can stay on top of home care tasks.
- **Acceptance Criteria**:
  - System checks maintenance schedules regularly.
  - Reminders are triggered before due dates.
  - User can configure how and when reminders are sent (e.g., email, push notification, in-app alert).

## Project Plan

###  Milestone 1: Initial System Design
 * Define features: e.g., track rooms, appliances, maintenance tasks
 * Draw architecture diagram (see next step)
 * Pick tech stack (Flask + PostgreSQL + HTML/CSS OR React)

### Milestone 2: Backend API
 * Set up Flask or FastAPI
 * Create CRUD endpoints for rooms/appliances/tasks
 * Add unit tests
 * Connect to local PostgreSQL DB

### Milestone 3: Frontend
 * Create simple web UI (HTML/React)
 * Connect forms to API
 * Style the UI (optional)

### Milestone 4: Deploy to AWS (MVP)
 * Provision EC2 instance or use Elastic Beanstalk
 * Install backend/frontend + DB on AWS
 * Add a domain + HTTPS via Route53 + ACM
 * Add logging/monitoring with CloudWatch

### Milestone 5: Dockerization
 * Dockerize backend & frontend
 * Use Docker Compose locally
 * Push images to Docker Hub or ECR

### Milestone 6: Kubernetes (Optional but Educational)
 * Set up local minikube or EKS cluster
 * Deploy using Helm or YAML files
 * Test scaling + rolling updates

### Milestone 7: Mobile App (Stretch Goal)
 * Set up React Native
 * Connect to API
 * Deploy to emulator or device# home-manager-cloud
