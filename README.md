# day-progress
This web app shows you your day as a progress bar of 1,440 minutes, color coded to show daylight vs nighttime.

## Current functionality
- Visually represents how much of the day had passed and shows current minute
- Tracks time passed minute to minute live
- Shows local sunrise and sunset times, automatically updated and adjusted daily
- Choose your location with ?location= query string in url. Saves this in local storage
- Switch to light theme with "?theme=light" in url. Defaults to dark theme if query string isn't present

## Bugs
- Closing app can get it out of sync. Test having something check and resync time every time you open it (assign “i” to a data attribute for each div and check against this?)
- Make the animating time passed optional, i.e. it only happens when you first open the app up, not if you need to resync the time
- Adjusts sunrise and sunset duration to location but shows that (and current time) in device timezone, not timezone at location
- Location lookup currently exposes location API, use netlify function instead
- Browser chrome on mobile causes vertical scroll, can’t see all minutes at once
- Between sunset and midnight, the "% of daylight minutes left" shows a negative percentage - ✅ 1/8/23

## To add
- % of daylight minutes left - ✅ 12/29/22
- Number of daylight minutes (% of day)
- Sunrise time
- Sunset time
- Minute progress bar

## Preference settings to add
- Show and set location in settings
- hide hour labels
- Increase contrast
- Change theme - ✅ 12/29/22
- Customize colors of individual elements 

## Misc
- Put these to-do’s somewhere public like the GitHub read me - ✅ 1/8/23
- Code it in Swift so it can be an iOS widget 😍😍😍😍

# Changelog
- 12/24/22
  - Created repo
- 12/25/22
  - Basic functionality
- 12/29/22
  - Add light theme 
  - Add progress bar to menu showing % of daylight minutes left + other stats
  - Add google analytics