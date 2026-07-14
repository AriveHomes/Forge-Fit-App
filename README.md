# ForgeFit Studio 7.0

A mobile-first workout and cardio Progressive Web App designed for GitHub Pages.

## Included

- Professional dashboard with readiness score and realistic muscle-recovery map
- Recovery-based workout recommendations with manual muscle selection
- 80-exercise starter database with equipment filters and search
- Add custom exercises, images, instructions, cues, demo-video files, or demo-video URLs
- Exercise form guides and motion previews
- AI Form Check beta using MediaPipe Pose Landmarker in the browser
- Add, switch, and delete user profiles
- Strength workout logging, sets, reps, weight, RPE, and rest timer
- Cardio logging for treadmill, running, bike, stair climber, elliptical, and rowing
- Progress charts, workout history, equipment setup, and data export

## Upload to GitHub Pages

1. Remove the files from the old ForgeFit repository, or create a fresh repository.
2. Upload `index.html` to the repository root. You can also upload this README and the preview image.
3. Commit the files.
4. Open **Settings → Pages**.
5. Under **Build and deployment**, select **Deploy from a branch**.
6. Select `main` and `/root`, then save.
7. Open the GitHub Pages address with `?v=7.0` appended once, for example:
   `https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/?v=7.0`

This version does not install a service worker, so it will not keep serving an older cached build.

## AI Form Check

Open an exercise, tap **AI Form Check**, and record or select a video. Keep your full body and the weight visible from the side or a 45-degree angle.

The feature loads MediaPipe Pose Landmarker from the internet, samples frames locally in the browser, estimates joint positions and range of motion, and returns exercise-specific coaching tips. The video is not uploaded to a ForgeFit server by this build. The feature is a beta training aid and is not a replacement for a qualified coach or medical professional.

## Exercise videos

Custom exercises can store a video selected from the phone or use a video URL. Built-in exercises currently use realistic still images and a motion-preview effect. A commercial App Store release should use original or properly licensed demonstration videos rather than copying footage from another fitness app.

## Storage

Profiles, workouts, settings, custom exercises, and custom exercise videos are stored locally in the browser on the device. A commercial multi-device version would need secure authentication and cloud storage.
