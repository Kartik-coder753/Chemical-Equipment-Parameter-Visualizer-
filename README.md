ChemEquip Visualizer 🔬📊
A high-performance dashboard for visualizing and analyzing chemical equipment parameters from CSV datasets, featuring AI-powered operational insights and automated PDF reporting.

🌟 Features
📈 Real-time Data Visualization: Interactive charts and graphs for equipment parameters
 
🤖 AI-Powered Insights: Gemini AI integration for operational recommendations

📊 Comprehensive Analytics: Summary statistics and type distribution analysis

📁 CSV Import: Upload and parse equipment data from CSV files

📄 PDF Reporting: Generate and export detailed analysis reports

📚 Session History: Store and reload previous analysis sessions

🔐 User Authentication: Secure login system for enterprise use

📱 Responsive Design: Works on desktop and mobile devices

🛠️ Tech Stack
Frontend: React 19, TypeScript, Vite

UI Components: Recharts, Lucide React, Tailwind CSS

AI Integration: Google Gemini API (@google/genai)

Data Visualization: Recharts

Build Tool: Vite

🚀 Quick Start
Prerequisites
Node.js 18.0 or higher

A Gemini API key from Google AI Studio

Installation
Clone the repository

bash
git clone <repository-url>
cd copy-of-chemequip-visualizer
Install dependencies

bash
npm install
Set up environment variables

Copy .env.local.example to .env.local (if exists) or create a new .env.local file

Add your Gemini API key:

env
VITE_GEMINI_API_KEY=your_actual_api_key_here
Start the development server

bash
npm run dev
Open your browser and navigate to http://localhost:3000

📁 Project Structure
text
copy-of-chemequip-visualizer/
├── src/
│   ├── components/          # React components
│   │   ├── Dashboard.tsx    # Main dashboard with charts
│   │   ├── Layout.tsx       # Application layout with sidebar
│   │   ├── Login.tsx        # Authentication component
│   │   └── HistoryView.tsx  # Session history view
│   ├── services/           # Business logic services
│   │   ├── dataService.ts  # CSV parsing and data utilities
│   │   └── geminiService.ts # Gemini AI integration
│   ├── types.ts            # TypeScript type definitions
│   └── App.tsx             # Main application component
├── public/                 # Static assets
├── index.html             # Main HTML entry point
├── vite.config.ts         # Vite configuration
├── tsconfig.json          # TypeScript configuration
└── package.json           # Dependencies and scripts
🔧 Configuration
Gemini API Setup
Obtain an API key from Google AI Studio

Update the .env.local file with your key

Restart the development server for changes to take effect

Sample Data Format
The application expects CSV files with the following columns:

csv
Equipment Name,Type,Flowrate,Pressure,Temperature
Heat Exchanger 01,Exchanger,450.5,12.5,85.2
Distillation Column A,Tower,1200.0,4.2,165.0
📊 Usage
Login: Use the default credentials (Admin/password) or implement your own authentication

Upload Data: Drag-and-drop a CSV file or use the sample dataset

Analyze: View interactive charts and AI-generated insights

Export: Generate PDF reports for documentation

History: Access previous analysis sessions from the history panel

🤖 AI Insights
The application uses Google's Gemini 1.5 Flash model to provide:

Operational risk assessments (Low/Medium/High)

Technical recommendations

Equipment performance observations

Maintenance suggestions

🐛 Troubleshooting
Common Issues
"No insights available for this dataset"

Verify your Gemini API key is correctly set in .env.local

Check browser console for error messages

Ensure you have an active internet connection

"Cannot find property 'VITE_GEMINI_API_KEY'"

Restart the development server after editing .env.local

CSV parsing errors

Ensure your CSV follows the required format

Check for missing or malformed columns

Chart rendering issues

Clear browser cache

Verify all dependencies are installed correctly

Debugging
Check the browser console for:

✅ Success messages

❌ Error indicators with emoji

Detailed error descriptions

📝 Scripts
npm run dev - Start development server

npm run build - Build for production

npm run preview - Preview production build

🔒 Security Notes
Never commit .env.local to version control

The demo uses localStorage for session history (not suitable for production)

Implement proper authentication for enterprise use

Consider adding HTTPS in production

🌐 Browser Support
Chrome 90+

Firefox 88+

Safari 14+

Edge 90+

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

🤝 Contributing
Fork the repository

Create a feature branch

Commit your changes

Push to the branch

Open a Pull Request

🙏 Acknowledgments
Google Gemini API for AI capabilities

Recharts for data visualization

Lucide Icons for beautiful icons

Tailwind CSS for styling

📧 Support
For issues, questions, or feature requests, please open an issue on the GitHub repository.

Happy Analyzing! 🧪📈


