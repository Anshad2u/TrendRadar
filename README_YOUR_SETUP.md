# Your TrendRadar Setup - Anshad2u

## 🎉 Setup Complete!

Your TrendRadar has been successfully configured with:

### ✅ What's Already Set Up

1. **Repository**: `Anshad2u/TrendRadar` (forked from sansan0/TrendRadar)
2. **GitHub Secrets Configured**:
   - `ENABLE_CRAWLER`: `true` (news crawling enabled)
   - `ENABLE_NOTIFICATION`: `true` (notifications enabled)
   - `REPORT_MODE`: `daily` (daily summary mode)
   - `AI_PROVIDER`: `openrouter` (OpenRouter AI service)
   - `AI_API_KEY`: Your OpenRouter API key (secured)
   - `TELEGRAM_BOT_TOKEN`: Your Telegram bot token (secured)
   - `TELEGRAM_CHAT_ID`: Placeholder (you'll set this next)

3. **Custom Configuration Files**:
   - `config/frequency_words.txt`: English keywords for tech/AI/business news
   - `config/ai_analysis_prompt.txt`: Custom AI analysis prompt in English
   - `config/config.yaml`: Customized with English interface, UTC timezone, tech platforms

4. **AI Model**: Xiaomi MiMo-V2-Flash (free model)

### 📋 Next Steps

#### Step 1: Get Your Telegram Chat ID

1. Open Telegram and search for `@Checktrends_bot` (your bot)
2. Start a chat with the bot by sending `/start`
3. Add the bot to a group or send it a message
4. Get your chat ID:
   - **Option A**: Use a bot like `@userinfobot` - send `/start` and it will show your chat ID
   - **Option B**: If in a group, the group ID is your chat ID (starts with `-`)
   - **Option C**: Send any message to your bot, then check the bot's updates

5. Add the chat ID to GitHub Secrets:
   - Go to: `https://github.com/Anshad2u/TrendRadar/settings/secrets/actions`
   - Find `TELEGRAM_CHAT_ID`
   - Click "Update" and paste your chat ID

#### Step 2: Test Your Setup

1. Go to your repository: `https://github.com/Anshad2u/TrendRadar`
2. Click on **Actions** tab
3. Find **"Get Hot News"** workflow
4. Click **"Run workflow"** button
5. Wait 3-5 minutes
6. Check your Telegram for test notifications

#### Step 3: Customize Further (Optional)

**Add More Keywords**:
- Edit `config/frequency_words.txt` in your repository
- Add your specific interests (cybersecurity, robotics, quantum computing, etc.)
- Commit the changes

**Change Report Mode**:
- Edit `config/config.yaml`
- Change `report.mode` to:
  - `"daily"` - Daily summary (all news of the day)
  - `"current"` - Current trending (real-time)
  - `"incremental"` - Only new news (no repeats)
- Commit the changes

**Add More RSS Feeds**:
- Edit `config/config.yaml`
- Add more RSS feeds under `rss.feeds` section
- Commit the changes

**Change AI Model**:
- Edit `config/config.yaml`
- Change `ai_analysis.model` to another OpenRouter model
- Examples: `"x/miMo-v2-flash"`, `"deepseek/deepseek-chat"`, `"google/gemini-2.0-flash-exp"`
- Commit the changes

### 🔧 Configuration Reference

#### Available Platforms (in config.yaml)
- Hacker News
- Reddit r/technology
- Product Hunt
- GitHub Trending
- TechCrunch
- Wired
- The Verge
- Ars Technica
- Engadget
- Mashable
- VentureBeat
- TechRepublic

#### Available RSS Feeds (in config.yaml)
- Hacker News (https://hnrss.org/frontpage)
- TechCrunch (https://techcrunch.com/feed/)
- Wired (https://www.wired.com/feed/rss)

#### AI Analysis Modes
- `original` - Only push original news
- `analysis` - Only push AI analysis
- `both` - Push both (recommended)

### 📊 Monitoring Your Setup

**Check Workflow Status**:
- Go to: `https://github.com/Anshad2u/TrendRadar/actions`
- View workflow runs and logs

**View Generated Reports**:
- Go to: `https://github.com/Anshad2u/TrendRadar/actions`
- Click on a completed workflow run
- Download artifacts (HTML reports)

**Check Activity**:
- GitHub Actions requires periodic check-ins (every 7 days)
- You'll receive reminders in Telegram
- To check in: Go to Actions → "Check In" → Run workflow

### 🚨 Important Notes

1. **Security**: Your API keys and tokens are stored securely in GitHub Secrets
2. **Privacy**: Your notifications go only to your Telegram chat
3. **Cost**: Using Xiaomi MiMo-V2-Flash (free model) - no API costs
4. **Rate Limits**: GitHub Actions has usage limits (check GitHub's documentation)
5. **Data Storage**: Data is stored locally in your repository (no cloud storage needed)

### 🆘 Troubleshooting

**No Telegram Messages**:
- Verify bot token is correct in GitHub Secrets
- Verify chat ID is correct in GitHub Secrets
- Check bot is not blocked in Telegram
- Try running workflow manually again

**AI Analysis Not Working**:
- Verify OpenRouter API key is correct
- Check if Xiaomi MiMo-V2-Flash is available in your region
- Try a different model in config.yaml

**Workflow Fails**:
- Check workflow logs for error messages
- Verify all secrets are set correctly
- Ensure your bot is active and not rate-limited

### 📞 Support

For issues with the original TrendRadar project:
- GitHub Issues: https://github.com/sansan0/TrendRadar/issues
- Documentation: https://github.com/sansan0/TrendRadar/blob/master/README.md

### 🎯 Your Customization

Your setup is configured with:
- ✅ English interface (no Chinese text)
- ✅ Tech/AI/Business focused keywords
- ✅ Telegram notifications
- ✅ AI analysis with Xiaomi MiMo-V2-Flash
- ✅ GitHub Actions deployment
- ✅ Custom platform list (international tech sources)

Enjoy your personalized TrendRadar! 🚀

---

**Quick Start Checklist**:
- [ ] Get Telegram Chat ID
- [ ] Add Chat ID to GitHub Secrets
- [ ] Run manual test workflow
- [ ] Verify Telegram notification received
- [ ] Customize keywords if needed
- [ ] Set up automatic schedule (default: every hour)

