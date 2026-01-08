🌉 Samartha Setu - Real-time Hyperlocal Food Sharing Platform
Symbolizing the Ram Setu — connecting donors and receivers across India in a lasting, reliable bridge.

"The food you save today might save a life tomorrow."
Samartha Setu is a full-stack MERN application that connects food donors with receivers to minimize food waste through real-time, hyperlocal matching. Built for hackathons with production-ready features.

Platform Name: Samartha Setu 
Meaning: A bridge of capability and compassion, inspired by the legendary Ram Setu that connected lands and hearts.

🎯 Core Features
✅ Implemented Features
**Authentication & Authorization**
JWT-based authentication
Role-based access control (Donor, Receiver, Admin)
Organization verification workflow
Secure password hashing with bcrypt

**Food Listing Management**
Create quick/bulk listings with geolocation
TTL-based automatic expiration (configurable)
Claim → Confirm → Complete workflow
Fallback routing (Receiver → Animal Farm → Biocompost)
Real-time status updates via Socket.IO

**Map Interface**
Leaflet.js + OpenStreetMap integration
Live pins for listings, fridges, animal farms, biocompost centers
Geospatial queries (radius-based filtering)
Food type and immediate pickup filters
Interactive popups with claim buttons

**Real-time Features**
Socket.IO for instant notifications
Live listing updates
Per-listing chat with quick replies
Claim/confirm/complete events
New message notifications

**Gamification & Leaderboard**
Points system (10 points per KG donated)
Automatic badge awards (5 tiers)
Public leaderboard with rankings
Reward eligibility tracking
Gift/certificate issuance

**Admin Panel**
Dashboard with analytics charts
User management (verify/ban)
Organization verification
Checkpoint management (fridges, animal farms, biocompost)
Reward creation and tracking
CSV export for listings/users

**Fallback Automation**
Cron-based TTL checking (runs every minute)
Auto-routing to nearest checkpoint if no claims
Configurable fallback delay
Checkpoint capacity tracking

**Ratings & Moderation**
Post-pickup ratings (1-5 stars)
Auto-ban for donors with low ratings (<2 stars, 5+ ratings)
Manual ban/unban by admins
Feedback collection

**🛠️ Tech Stack**
**Backend**
Node.js + Express.js
MongoDB with Mongoose (geospatial indexes)
Socket.IO for real-time communication
JWT for authentication
bcrypt for password hashing
node-cron for TTL automation
express-rate-limit for API protection
helmet + CORS for security

**Frontend**
React 18 with Hooks
React Router v6 for routing
Axios for API calls
Socket.IO Client for real-time updates
Leaflet + React-Leaflet for maps
Lucide React for icons
React Hot Toast for notifications
date-fns for date formatting

