💣 Ticking Bomb – Idea Igniter App
Where ideas are born fast... or fade into beautiful memories.
Act quickly, or your imagination turns into a vintage postcard on the Wall of Procrastination.

🛠 Built with
- Windsurf (frontend + backend actions)
- Vercel (deployment)
- Supabase (database + storage)
- OpenAI API (for idea scoring)
- DALL·E API (optional: generate lost idea postcards)

📦 Project Structure
Folders:
- /app/new — Page to dump new ideas
- /app/wall — Wall of Procrastination (gallery of detonated ideas)
- /app/graveyard — View dead/lost ideas individually
- /db — Supabase schema for ideas table
- /gpt_actions/score_idea.ts — OpenAI API action for idea scoring
- /gpt_actions/postcard_prompt.ts — (optional) OpenAI API action for postcard generation
- /public/assets/stamps — Visual stamps (Fire, High, Mid Potential)
- /public/assets/textures — Vintage paper textures for aging effect

⚡ Quick Setup Instructions
1. Clone the repo:
git clone https://github.com/YOUR_USERNAME/ticking-bomb.git
cd ticking-bomb

2. Install dependencies:
pnpm install

3. Set up environment variables:
Create a .env file and add:
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
OPENAI_API_KEY=your_openai_key

4. Deploy database schema:
- Create a Supabase project.
- Run the SQL inside /db/schema.sql to create the ideas table.

5. Run your project locally:
pnpm dev

6. Deploy to Vercel:
- Push to GitHub
- Connect the repo to Vercel
- Deploy

🚀 Core Features
- Submit random ideas
- AI evaluates and scores the idea
- Assigns Fire/High/Mid Potential stamp
- Countdown ticking timer on each idea
- Visual "aging" as timer runs out
- Graveyard view for detonated ideas
- (Optional) AI-generated vintage postcards for dead ideas
- Wall of Procrastination gallery
- (Stretch goal) Shareable public wall link

📚 API Actions
- /gpt_actions/score_idea.ts: Sends idea to OpenAI and returns score, stamp, and reason
- /gpt_actions/postcard_prompt.ts: (Optional) Sends detonated idea to DALL·E to create a vintage postcard

🎨 Visual Ingredients
- 3 Potential Stamps:
🔥 Fire Potential
⚡ High Potential
💭 Mid Potential
- Vintage paper textures
- CSS filters for aging effect (sepia, brightness decay, etc.)

All visuals live inside /public/assets/.

✨ Future Ideas
- Trophies for saving ideas before detonation
- AI-generated tiny poetic obituaries for lost ideas
- Collaborator Walls (share graveyards between friends)
- Auto-post detonated postcards to social media

🧠 Philosophy
Don’t just collect ideas.
Feel the urgency to bring them to life — or honor them when they pass.

📸 Preview
(Add a screenshot of your Wall of Procrastination here once it's live!)

🐣 License
MIT License.
Build responsibly and creatively.

🙌 Acknowledgements
Thanks to OpenAI, Supabase, Windsurf, and all relentless idea-makers.

📈 Quick Dev Notes
- Focus on shipping end-to-end flows with fake data first.
- Once UX feels alive, plug in OpenAI and Supabase.
- Launch early, polish later. This app shines because of the emotional experience, not feature overload.

🎯 TL;DR
Build fast. Ship magic. Honor your dead ideas.