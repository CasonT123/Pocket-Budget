POCKET BUDGET — INSTALL ON IPHONE

This is a small private budgeting web app. It does not connect to a bank.

FIRST: PUT IT ON A SECURE WEBSITE
Option A — GitHub Pages (free)
1. Create a new PUBLIC repository at github.com named pocket-budget.
2. Upload the contents of this ZIP (index.html, manifest.webmanifest, sw.js, icons) to the repository root. Do NOT upload the enclosing folder without moving files to root.
3. Go to repository Settings > Pages > Build and deployment > Deploy from a branch. Choose main and /(root). Save.
4. Open the resulting https://YOUR-USERNAME.github.io/pocket-budget/ URL in Safari on your iPhone. It may take time for the website to be published.
5. In Safari, tap Share > Add to Home Screen > Add. You can now launch it as an app.

Option B — Any static web host supporting HTTPS works (Netlify Drop, Cloudflare Pages, etc.).

HOW IT WORKS
- Enter each purchase or savings transfer by tapping Add expense or transfer.
- Set category percentages once. New paychecks automatically scale the category budgets to your actual income.
- On payday tap New paycheck, enter the actual amount, and start a new two-week period.
- Look at history or export a JSON backup in Settings.

IMPORTANT NOTES
- Only spend money from a category once: withdrawing cash isn't the same as spending it.
- Subscription target $20 per two-week paycheck may need a little adjustment depending on the actual amount charged.
- Percentages must add up to 100%. Money is distributed to the nearest cent.
- Savings is counted as money moved out of the spendable paycheck; record it when you actually transfer it.
- This app stores data using browser localStorage ON THIS DEVICE. It does not sync with other devices and is not as durable as a server-backed app. Clearing Safari website data, some device migrations, or changing the hosted URL can erase the records. Export a backup regularly.
- Avoid uploading exported backups to public GitHub repositories.
- For an updated version, replace the hosted files. Some browsers may keep old files cached; bump the cache name in sw.js for major updates.

VERSION 3 UPDATE
- Savings total now leads the dashboard, summing savings transfers across all paychecks saved on this device.
- Set an editable savings goal via Edit goal. Goal progress is measured against recorded savings transfers, not a real bank account balance.
- The current paycheck remaining amount is shown in a secondary card.
- If upgrading the same hosted URL, replace the existing files and keep the same domain/path to retain local data. Export a backup before upgrading.
