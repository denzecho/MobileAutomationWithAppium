Run test:
- npm run test

Find appActivity and appPackage
- open app first, and leave in first screen / home screen
- run command: adb shell dumpsys activity activities | findstr "ResumedActivity"
  - example output:  ResumedActivity: ActivityRecord{f438f57 u0 com.miui.calculator/.cal.CalculatorActivity}
  - appPackage = com.miui.calculator
  - appActivity = .cal.CalculatorActivity