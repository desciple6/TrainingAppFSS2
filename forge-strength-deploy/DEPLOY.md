# Forge Strength Systems - Vercel Deployment Guide

## 🚀 Quick Deploy (5 minutes)

### Step 1: Download & Extract
Download the `forge-strength-deploy` folder to your computer.

### Step 2: Deploy to Vercel

**Option A: Using Vercel CLI (Recommended)**
```bash
# Install Vercel CLI (one-time setup)
npm install -g vercel

# Navigate to the project folder
cd forge-strength-deploy

# Deploy
vercel

# Follow the prompts:
# - Link to existing project? N
# - Project name: forge-strength-systems (or your choice)
# - Directory: ./ (press enter)
# - Want to modify settings? N
```

**Option B: Using Vercel Dashboard**
1. Go to https://vercel.com (sign up if needed - it's free!)
2. Click "Add New Project"
3. Click "Import Third-Party Git Repository" OR drag the folder
4. Select the `forge-strength-deploy` folder
5. Click "Deploy"
6. ✅ Done! Your app will be live in ~60 seconds

### Step 3: Custom Domain (Optional)
1. In Vercel dashboard, go to your project
2. Click "Settings" → "Domains"
3. Add your domain (e.g., `app.forgestrength.com`)
4. Follow Vercel's DNS setup instructions

---

## 📱 Features Included

✅ **Federation & Equipment Selection**
- USAPL, IPF, USPA, WRPF, RPS, SPF, and 15+ federations
- Raw vs Equipped tracking

✅ **OpenPowerlifting Integration**
- Search athletes by name
- View complete meet history
- See squat/bench/deadlift/total from each meet
- DOTS scores and placements

✅ **IPF World Records Comparison**
- Auto-calculated for client's weight class
- Age class based (Open, Junior, Masters, etc.)
- Equipment-specific records

✅ **Complete Client Stats**
- Personal: Sex, Age, Height, Bodyweight
- Training: Years experience, days/week
- Recovery: Diet, Sleep, Stress, Recovery (1-5 scales)
- Weak points: Squat, Bench, Deadlift positions

✅ **MEV/MRV Auto-Calculation**
- Personalized volume targets
- Based on recovery factors, experience, sex, bodyweight
- Adjusts per phase (Hypertrophy/Strength/Peaking)

✅ **Analytics Dashboard**
- Fatigue score (0-100)
- Recovery recommendations
- Weekly trends (RPE, difficulty, completion)
- Total volume by lift

✅ **Program Management**
- 16-week programs
- Auto-calculated loads from 1RMs
- Copy weeks for progressive overload
- Exercise library

✅ **Workout Logging**
- RPE tracking (0-10 scale)
- Difficulty ratings (1-5)
- Sets completed
- Persistent data storage

---

## 🔐 Login Codes

**Coach Dashboard:**
- Code: `COACH`

**Demo Client:**
- Code: `1234`

**Add New Clients:**
1. Login as coach
2. Click "+ ADD NEW CLIENT"
3. Enter client details
4. Share the generated code with your client

---

## 💾 Data Storage

- Uses browser localStorage
- Data persists across sessions
- No backend database needed (keeps it simple & free!)
- Each client's data is stored separately

---

## 🎨 Branding

The app uses:
- **Colors:** Black background, Red accents (#DC2626)
- **Font:** JetBrains Mono (loaded from Google Fonts)
- **Theme:** Brutalist/Industrial design

To customize:
- Edit colors in `tailwind.config.js`
- Update logo in `public/` folder
- Modify styles in `styles/globals.css`

---

## 🛠️ Local Development

```bash
# Install dependencies
npm install

# Run development server
npm run dev

# Open http://localhost:3000
```

---

## 📊 How to Use

### As a Coach:
1. Login with `COACH`
2. Click "+ ADD NEW CLIENT"
3. Fill in client stats (federation, equipment, 1RMs, etc.)
4. Click "CLIENT STATS" to edit full profile
5. Click "COMP HISTORY" to search OpenPowerlifting
6. Click "EDIT PROGRAM" to customize their training
7. View MEV/MRV targets on each client card

### As a Client:
1. Login with your coach-provided code
2. Select your week and training day
3. Log your workouts:
   - Enter sets completed
   - Rate RPE (how hard it felt, 0-10)
   - Rate difficulty (1-5)
   - Click "MARK COMPLETE"
4. Click "ANALYTICS" to view:
   - Your fatigue score
   - Recovery status
   - Weekly trends
   - Total volume

---

## 🔄 Updates

To update the app:
```bash
# Make your changes
# Then redeploy
vercel --prod
```

---

## 📧 Support

For issues or questions:
- Check the console (F12) for error messages
- Ensure you're using a modern browser (Chrome, Firefox, Safari, Edge)
- Clear browser cache if data seems stuck

---

## ✅ Success Checklist

After deployment:
- [ ] App loads at your Vercel URL
- [ ] Can login as COACH
- [ ] Can add a new client
- [ ] Can edit client stats
- [ ] Can search OpenPowerlifting
- [ ] Can edit programs
- [ ] Client login works
- [ ] Workout logging works
- [ ] Analytics display correctly
- [ ] Data persists after refresh

**Your app is ready to use! 🎉**

Share your Vercel URL with clients and start coaching!
