# PTO planner

Plan your time off from **December 2026 through December 2027**. The planner shows US holidays, points out the days that turn into long breaks, and lets you sketch a few versions of your plan.

**Try it:** https://sonal-dezign.github.io/pto-planner/

## Features

- **US holidays.** All 11 federal holidays plus New Year's Eve are shown, and holidays that fall on a weekend move to the observed weekday. Your company doesn't give you Columbus Day? Click **Edit holidays** to change any holiday, or add your own company holidays.
- **Smart picks.** A dashed outline marks the one weekday next to each holiday that turns it into a 4-day weekend. For example, take Fri, Nov 26, 2027 for Thursday–Sunday off over Thanksgiving.
- **Auto-plan.** Enter how many days off you have (PTO plus any floating holidays), and one click places them where it gets you the most days off and spreads your breaks through the year.
- **Office days.** Mark the days you'll be in the office if you work hybrid.
- **Work abroad (optional).** If your company lets you work from another country for a set number of days, enter that number in Settings and mark those days. They don't use PTO.
- **Cycle days (optional, off by default).** Mark the days you expect your cycle, so your trips don't overlap with them. They stay private, and are never included in share links. You can delete them anytime in Settings.
- **Up to 8 plans.** Sketch different versions, like "Beach week" or "Visiting family", and rename them anytime.
- **Share link.** Send a plan to your partner or friends. It opens as a new option in their planner.
- Follows your device's light or dark mode, and works on phones.

## Privacy

There are no accounts, no tracking and no server. Your plans are saved in your browser (`localStorage`) and never leave your device unless you share a link.

## Host your own copy on GitHub Pages

1. Create a new public repository named `pto-planner`.
2. Upload `index.html` and `README.md` to it.
3. Go to **Settings → Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, choose `main` and `/ (root)`, then click **Save**.
4. After a minute or two, your planner is live at `https://<your-username>.github.io/pto-planner/`.

## Roll it forward to another year

Open `index.html` and change these lines near the top of the script:

```js
const START_Y = 2026, START_M = 11;   // December 2026 (months are 0-based, so 11 = December)
const END_Y   = 2027, END_M   = 11;   // December 2027
```

US holidays are calculated automatically for any year.

## License

MIT. Use it, fork it, make it yours.

Made by Sonal Jaiswal.
