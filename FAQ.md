# Trackless Links FAQ

**Frequently Asked Questions & User Guide**

Welcome! This guide will help you get the most out of Trackless Links and answer common questions.

---

## Background: Why Clean URLs Matter

When Tim Berners-Lee invented the World Wide Web in 1989, URLs were designed to be simple addresses: a way to find a document on a server. A URL like `shop.com/shoes` told you exactly where you were going.

Today, URLs have become surveillance tools.

### The Hidden Economy of Your Clicks

Every time you click a link in an email, tap a post on social media, or follow a search result, extra code gets attached to the URL. These tracking parameters turn a simple address into a detailed report about you:

```
shop.com/shoes?utm_source=newsletter&utm_campaign=spring_sale&utm_medium=email&fbclid=IwAR3x...&mc_eid=abc123
```

This single URL tells multiple companies:
- You came from an email newsletter (not the website directly)
- You responded to the "spring sale" campaign
- Facebook knows you clicked this specific link
- The email marketing platform logged your unique subscriber ID

None of this affects what page you see. It only affects what companies learn about you.

### How Tracking Parameters Work

The question mark (?) in a URL separates the page address from its parameters. Everything after the question mark is metadata, and companies have standardized this into a surveillance system:

| Parameter | Who uses it | What it reveals |
|-----------|-------------|-----------------|
| `utm_source` | Marketers everywhere | Which website or platform sent you |
| `utm_campaign` | Marketers everywhere | Which specific ad or email you clicked |
| `fbclid` | Facebook/Meta | Your Facebook user ID and click behavior |
| `gclid` | Google | Your Google advertising profile |
| `mc_eid` | Mailchimp | Your email subscriber identity |
| `ttclid` | TikTok | Your TikTok advertising profile |
| `msclkid` | Microsoft/Bing | Your Microsoft advertising profile |

When you share a link with friends, you often share these parameters too, letting companies track not just you, but everyone who clicks the link you forwarded.

### The Privacy Cost

This tracking happens invisibly, but the consequences are real:

**Cross-site profiling**: Companies like Facebook and Google see your activity across millions of websites, building detailed profiles of your interests, purchases, and habits.

**Price discrimination**: Some retailers use tracking data to show different prices to different users based on their perceived willingness to pay.

**Filter bubbles**: Ad platforms use your click history to decide what content you see, potentially limiting your exposure to diverse viewpoints.

**Data breaches**: Every company storing your tracking data is a potential breach target. The less data collected, the less can be stolen.

### What Trackless Links Does

Trackless Links intercepts URLs before they load and strips out tracking parameters. The cleaned URL still takes you to the same page, but without broadcasting your digital fingerprint.

Before: `amazon.com/dp/1119737281?tag=influencer-20&ref=pd_sl_abc&utm_source=instagram`

After: `amazon.com/dp/1119737281`

This happens automatically for every link in Safari, restoring URLs to what they were meant to be: simple addresses, nothing more.

---

## Getting Started

### How do I enable the Safari extension?

After installing the app:

1. Open **Safari** on your device
2. Tap the **AA** icon (or **Extensions** button on Mac) in the address bar
3. Tap **Manage Extensions**
4. Find **Trackless Links** and toggle it **on**
5. Grant the necessary permissions

The extension is now active and will start cleaning URLs automatically.

### Why isn't the extension working?

Make sure you have:
- Enabled the extension in Safari settings (see above)
- Granted the required permissions when prompted
- The extension needs permission to access web page content to function

On Mac, you may also need to check **System Settings > Privacy & Security > Extensions** and enable Trackless Links.

### Do I need to configure anything to start using it?

No. Trackless Links works out of the box with sensible defaults:
- Tracking parameters are automatically removed
- 20+ predefined redirects are ready to use (you can enable the ones you want)
- All tweaks are opt-in, so enable only what you need

---

## Privacy & Tracking Filters

### What tracking parameters does it remove?

Trackless Links removes common tracking codes like:
- `utm_source`, `utm_medium`, `utm_campaign` (marketing attribution)
- `fbclid` (Facebook click identifier)
- `gclid` (Google click identifier)
- `msclkid` (Microsoft/Bing click identifier)
- And dozens more

You can view the full list in the **Filters** tab and add your own custom parameters.

### How do I add a custom tracking parameter?

1. Open the Trackless Links app
2. Go to the **Filters** tab
3. Tap the **+** button
4. Enter the parameter name (e.g., `my_tracker`)
5. Tap **Save**

The next time you visit a URL with that parameter, it will be automatically removed.

### Can I temporarily disable tracking removal?

Yes. In the **Filters** tab, you can toggle individual filters on or off. You can also disable all tracking removal by turning off all filters.

---

## Redirects

### What are redirects and why would I use them?

Many popular websites collect extensive data about their users. Redirects let you automatically route yourself to privacy-respecting alternatives that provide the same content without the surveillance.

**Privacy-focused frontends**: Projects like Nitter (for Twitter/X), Invidious (for YouTube), and Libreddit (for Reddit) display content from major platforms without logging you in or tracking your behavior. You get the content, they don't get your data.

**Interface preferences**: Reddit's old.reddit.com provides the classic interface many users prefer. Some news sites have cleaner mobile versions. Redirects let you always land on your preferred version.

**Regional routing**: Automatically redirect international domains to your local version, or vice versa.

### How do I enable a predefined redirect?

1. Open the app and go to **Redirects**
2. Browse the list of predefined rules
3. Toggle the switch next to any rule to enable it
4. The redirect is active immediately, no restart needed

### How do I create a custom redirect?

1. Go to **Redirects** tab
2. Tap the **+** button
3. Enter:
   - **Pattern**: The URL you want to redirect FROM (e.g., `reddit.com`)
   - **Replacement**: Where to redirect TO (e.g., `old.reddit.com`)
   - **Title** (optional): A friendly name for this rule
4. Tap **Save**

You can use exact matches or regular expressions (regex) for advanced patterns.

### Can I reorder my redirect rules?

Yes. Order matters because the first matching rule wins. To reorder:

1. Go to **Redirects**
2. Long-press and drag rules to rearrange them
3. Your priority is saved automatically

### My redirect is not working. What is wrong?

Check these common issues:

- Is the rule **enabled**? (toggle switch is on)
- Is the pattern correct? (test with a simple exact match first)
- Is another rule matching first? (check rule order)
- Are you testing in Safari? (the extension only works in Safari, not other browsers)

---

## Tweaks

### What are tweaks?

Modern websites often restrict what you can do in your own browser. They disable text selection to prevent copying, autoplay videos to boost engagement metrics, and show intrusive popups to keep you from leaving.

Tweaks restore control to you:

- Re-enable text selection on sites that block it
- Block autoplay videos and audio
- Force dark mode on any website
- Remove "Are you sure you want to leave?" popups
- And more

All tweaks are opt-in, so you control which ones to enable.

### How do I enable tweaks?

1. Go to the **Tweaks** tab
2. Browse the available options
3. Toggle any tweak on or off
4. Changes apply immediately

### Why doesn't a tweak work on a specific site?

Some websites actively fight against modifications. If a tweak does not work:

- The site may be using aggressive anti-modification techniques
- Try disabling other extensions to rule out conflicts
- Report the issue on GitHub. We are always improving compatibility.

### What is the difference between "Force Media Controls" and "Block Autoplay"?

- **Force Media Controls**: Shows the standard browser video/audio controls even if the site hides them
- **Block Autoplay**: Prevents videos/audio from playing automatically when you load a page

You can use them together for maximum control.

---

## Archive Search

### What is Archive Search?

The web is not permanent. Pages get deleted, articles get edited, and entire websites disappear. The Internet Archive's Wayback Machine and similar services preserve snapshots of the web, creating a historical record of what existed at any given time.

Archive Search gives you instant access to these preserved versions:

- Find deleted content or see what a page looked like before it was changed
- Access pages when a site is temporarily down
- Research how websites and their claims have evolved over time
- Verify quotes and citations that may have been altered

### How do I search an archive?

**From Safari:**
1. Tap the **AA** icon or **Extensions** button
2. Select **Trackless Links**
3. Tap the archive service you want (e.g., Wayback Machine)
4. The current page will be searched in that archive

**From any app (Share Sheet):**
1. Share a link from any app
2. Choose **Search in Archive**
3. Select your preferred archive service

### Can I add more archive services?

Yes. You can add custom archive services:

1. Go to **Tweaks** then **Archive Search** then **Configure Services**
2. Tap **+** to add a service
3. Enter the archive service URL pattern
4. The service is now available in the popup

### Should I enable "Strip Query Parameters"?

Recommended: Yes. This option removes tracking codes and other parameters before searching archives, which often leads to better matches. Disable it only if you need to search for a URL with specific parameters intact.

---

## Share Sheet Integration

### How do I use the Share Sheet to clean links?

When you share links from other apps, tracking parameters come along for the ride. The Share Sheet extension lets you clean links before sharing them:

1. In any app (Safari, Reddit, X, etc.), tap the **Share** button
2. Scroll and find **Clean with Trackless Links**
3. The cleaned URL is copied to your clipboard

Now you can share a clean link that does not reveal where you found it or track everyone who clicks it.

### Can I share to archives from other apps?

Yes. Use the same Share Sheet:

1. Tap **Share** on any link
2. Choose **Search in Archive**
3. Select your archive service
4. Safari will open with the archive search results

---

## iCloud Sync

### How does iCloud sync work?

Your privacy settings travel with you. When you enable iCloud sync, your configuration syncs automatically across iPhone, iPad, and Mac via your personal iCloud account:

- **Filters** (tracking parameters)
- **Redirects** (custom rules and enabled state)
- **Tweaks** (all settings)
- **Archive services** (your configured services)

Privacy statistics (like your blocked tracker count) remain device-specific and do not sync.

### Do I need to enable iCloud sync?

It is optional. iCloud sync is disabled by default. To enable it:

1. Go to **Settings** in the app
2. Find **iCloud Sync**
3. Toggle it **on**

Your settings will now sync across all devices signed into the same iCloud account.

### My changes are not syncing between devices. What is wrong?

Check these:

- Is iCloud sync **enabled** on both devices?
- Are both devices signed into the **same iCloud account**?
- Is iCloud Drive enabled in **System Settings** (Mac) or **Settings** (iOS)?
- Are both devices connected to the internet?
- Try force-quitting and reopening the app

If sync still does not work, try toggling iCloud sync off and back on.

### Can I use Trackless Links without iCloud?

Yes. iCloud sync is completely optional. The app works perfectly fine storing all settings locally on each device.

---

## Tips & Tricks

### How can I see what tracking parameters were removed?

Check the **Statistics** on the main dashboard. It shows:
- Total URLs cleaned
- Redirects applied

### Can I export my settings?

Settings are stored in iCloud (if enabled) or locally on your device. All data remains under your control and is never sent to third-party servers.

### Does Trackless Links slow down browsing?

No. The extension is extremely lightweight and processes URLs in milliseconds before pages finish loading. You will not notice any performance impact.

### Can I use Trackless Links with other Safari extensions?

Yes. Trackless Links is designed to work alongside other extensions. If you experience conflicts, try adjusting the execution order in Safari's extension settings.

### What is the difference between Trackless Links and Trackless Links Pro?

| Feature | Trackless Links | Trackless Links Pro |
|---------|----------------|---------------------|
| iPhone and iPad | Yes | Yes |
| Mac app | No | Yes |
| iCloud sync | Yes | Yes |
| Pricing | One-time purchase (iOS only) | Universal purchase (all platforms) |

Trackless Links Pro is a universal purchase. Buy once and use on iPhone, iPad, and Mac.

---

## Troubleshooting

### I cannot find the extension in Safari

Make sure:
- You have installed the app from the App Store
- You have opened the app at least once
- Safari extensions are enabled in your system settings

### Links are not being cleaned

Check:
- Is the extension **enabled** in Safari?
- Did you grant the necessary permissions?
- Are there any filters **enabled** in the Filters tab?

### My custom redirect is not working

- Double-check the pattern syntax (try an exact match first)
- Make sure the rule is **enabled**
- Check that no other rule is matching first (rule order matters)
