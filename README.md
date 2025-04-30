# Real-time Traffic Detection System

A full-stack application for real-time traffic monitoring and analysis using machine learning. This project detects vehicles in video streams, classifies them, and provides comprehensive traffic statistics.

## Features

- **Real-time Traffic Monitoring**: Process live video feeds to detect and track vehicles
- **Vehicle Classification**: Identify different types of vehicles (cars, trucks, buses, motorcycles, etc.)
- **Traffic Statistics**: Generate detailed traffic analytics and visualizations
- **User Authentication**: Secure user accounts with JWT authentication
- **Responsive Dashboard**: Access traffic data from any device
- **Historical Data Analysis**: Review past traffic patterns and trends
- **Data Export**: Export traffic reports for further analysis

## Tech Stack

### Frontend
- React.js for the user interface
- Redux for state management
- Chakra UI for responsive design components
- Chart.js for data visualization
- React Router for navigation

### Backend
- Node.js and Express for the API server
- MongoDB for data storage
- JWT for authentication
- Multer for file uploads

### Machine Learning
- Python for ML processing
- OpenCV for image processing
- YOLOv3 for object detection (simulated in this demo)

## Installation and Setup

### Prerequisites
- Node.js (v14.0.0 or later)
- MongoDB
- Python 3.6+ (for ML component)

### Backend Setup
1. Clone the repository
```bash
git clone https://github.com/yourusername/traffic-detection-system.git
cd traffic-detection-system
```

2. Install backend dependencies
```bash
npm install
```

3. Configure environment variables
Create a `.env` file in the root directory with the following variables:
```
NODE_ENV=development
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

4. Start the backend server
```bash
npm run server
```

### Frontend Setup
1. Navigate to the frontend directory and install dependencies
```bash
cd frontend
npm install
```

2. Start the frontend development server
```bash
npm start
```

### ML Component Setup
1. Install Python dependencies
```bash
pip install opencv-python numpy
```

## Usage

1. Register for an account on the platform
2. Log in to access the dashboard
3. Navigate to the Detection page to start processing video feeds
4. View traffic statistics and historical data in the Dashboard and Statistics pages
5. Export reports as needed

## Project Structure

```
traffic-detection-system/
├── backend/               # Node.js server
│   ├── config/            # Database configuration
│   ├── controllers/       # Request handlers
│   ├── middleware/        # Authentication middleware
│   ├── models/            # Mongoose models
│   ├── routes/            # API routes
│   └── server.js          # Server entry point
├── frontend/              # React application
│   ├── public/            # Static files
│   └── src/               # React source code
│       ├── actions/       # Redux actions
│       ├── components/    # Reusable components
│       ├── constants/     # Action types
│       ├── reducers/      # Redux reducers
│       └── screens/       # Page components
├── ml/                    # Machine learning scripts
│   └── detector.py        # Traffic detection script
├── uploads/               # Uploaded images/videos
└── README.md              # Project documentation
```

## Future Enhancements

- **Real-time Notifications**: Alert system for unusual traffic patterns or incidents
- **More Advanced ML Models**: Implement more sophisticated detection algorithms
- **Traffic Prediction**: Forecast traffic patterns based on historical data
- **Mobile App**: Dedicated mobile application for on-the-go monitoring
- **Integration with Traffic Signals**: Connect with traffic management systems

## License

This project is licensed under the MIT License 
