# 🖱️ A Click That Talks Back

**An interactive automation experiment** that connects website user behavior to smart email workflows — powered by **Google Apps Script**, **Sheets**, and a **3D Spline demo**.

When a user clicks **“View Pricing”**, this system:

1. Increases their *Intent Score* in a connected Google Sheet
2. Updates their *Last Action* column
3. Sends a personalized, ready-to-send email draft with a 3D walkthrough link

All in a single click.

---

## ⚙️ How It Works

| Step | What Happens                 | Tools Used                                 |
| ---- | ---------------------------- | ------------------------------------------ |
| 1    | User clicks **View Pricing** | Front-end button with query param (email)  |
| 2    | Script receives the request  | Google Apps Script (doGet)                 |
| 3    | System finds matching lead   | Google Sheets lookup                       |
| 4    | Intent score increases       | Auto-calculated via Apps Script            |
| 5    | Rep receives email draft     | MailApp + dynamic message                  |
| 6    | Email includes 3D demo       | Hosted via [Spline](https://spline.design) |

---

## 🧠 Example Flow

### Before the Click

Spreadsheet looks like this:

```
Email                 | Intent Score | Last Action
-------------------------------------------------
zunigavanessa@smith.info |             |
```

### After the Click

```
Email                 | Intent Score | Last Action
-------------------------------------------------
zunigavanessa@smith.info | 40          | Viewed pricing page
```

### Auto Email Sent

```
Hi there,

Noticed you were exploring pricing. 
If you share how many users and your monthly print volume, 
I can confirm the best cost-efficient plan.

You can also explore a quick 3D walkthrough here:
https://my.spline.design/spline3dstarterfile-GGum3MrVqKm1QUATAtMKWOe3/

Would you like a 10-minute walkthrough?
```

---

## 🧩 Project Files

| File                  | Description                                                |
| --------------------- | ---------------------------------------------------------- |
| `Code.gs`             | Apps Script handling lookup, score update, and email draft |
| `customersjai.csv`    | Lead data sheet connected to the script                    |
| `spline3dstarterfile` | 3D product visualization built in Spline                   |
| `README.md`           | This documentation                                         |

---

## 🎨 3D Visualization

Built with **Spline (free version)**
Shows a **printer model** with floating text for ink optimization, cost-per-print, and AR-like perspective.

**Preview:**
![3D Printer](./sheet%205.png)

---

## 🚀 Why It Matters

* Shows **real-time intent tracking** without a CRM.
* Turns user curiosity into **automated, contextual outreach**.
* Demonstrates **marketing-tech workflow thinking** — from UX to backend.

---

## 💡 What’s Next

* Add webhook integration for HubSpot or Zapier
* Automate Slack alerts for high-intent leads
* Convert to Node.js backend for API-based scalability

---

## 🧍‍♂️ Author

**Purushotham Raju (Puru)**
Data + Design + Automation Enthusiast
📫 [LinkedIn](https://www.linkedin.com/in/purushothamraju) | 🌐 Fredericton, Canada

---

Would you like me to include your *distorted "View Pricing"* image and *email screenshot* as visual sections (like an “Interaction Flow” diagram) right inside the README layout next?
I can format it cleanly with `<img>` tags and proper spacing.
