# ⚡ Forge Strength Systems

**Professional Powerlifting Coaching Platform**

A complete web application for powerlifting coaches to manage clients, track progress, and integrate with OpenPowerlifting competition data.

## 🎯 Key Features

- **Federation & Equipment Tracking** - USAPL, IPF, USPA, and 15+ federations
- **OpenPowerlifting Integration** - Search athlete competition history
- **IPF World Records** - Auto-compare client lifts to world records
- **MEV/MRV Calculation** - Personalized volume targets
- **Analytics Dashboard** - Fatigue tracking and recovery metrics
- **Program Management** - 16-week customizable programs
- **Mobile Optimized** - Works perfectly on phones and tablets

## 🚀 Quick Start

See [DEPLOY.md](./DEPLOY.md) for complete deployment instructions.

```bash
npm install
npm run dev
```

Then open http://localhost:3000

## 🔐 Default Login

- **Coach:** `COACH`
- **Demo Client:** `1234`

## 📚 Tech Stack

- **Framework:** Next.js 14
- **Styling:** Tailwind CSS
- **Icons:** Lucide React
- **Deployment:** Vercel (recommended)
- **Storage:** Browser localStorage

## 📖 Documentation

- `DEPLOY.md` - Complete deployment guide
- `package.json` - Dependencies and scripts
- `pages/index.js` - Main application code

## 🏋️ For Coaches

- Manage unlimited clients
- Track client stats (age, sex, bodyweight, federation)
- Edit 16-week progressive programs
- View OpenPowerlifting competition history
- Monitor client compliance and fatigue
- Calculate MEV/MRV volume targets

## 📱 For Athletes

- Log workouts with RPE and difficulty ratings
- View personalized programs
- Track analytics and fatigue scores
- See volume recommendations
- Mobile-friendly interface

## 🎨 Customization

Edit these files to customize:
- `tailwind.config.js` - Colors and theme
- `styles/globals.css` - Global styles
- `pages/index.js` - Application logic

## 📊 Data Model

```javascript
Client {
  name, code, sex, age, height, bodyweight,
  squat_1rm, bench_1rm, deadlift_1rm,
  federation, equipment,
  yearsTraining, trainingDaysPerWeek,
  recoveryFactors: { diet, sleep, stress, recovery },
  weakPoints: { squat, bench, deadlift },
  currentWeek, currentPhase
}
```

## 🔄 Version History

- **v1.0.0** - Initial release with full feature set

## 📄 License

Built for Forge Strength Systems
