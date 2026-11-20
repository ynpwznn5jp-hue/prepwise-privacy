# Prepwise privacy policy

Last updated: November 20, 2026

Prepwise is a food tracking and meal prep app made by Chris Dunn. This page says plainly what it keeps, where, and why.

## On your phone
Your profile, food diary, saved foods, daily targets, recipes, grocery lists, pantry, prep plans and meal ratings are
stored on your iPhone. They stay there unless you choose to share something.

## If you sign in
Signing in with Apple is optional. It is needed to share a grocery list, to use Friends, and to use Prepwise's
Claude without a key of your own. When you sign in,
Prepwise stores, on a private database run on Supabase:

- your Apple account's user id, and the email address Apple provides (it may be a private relay address),
- the name and food emoji you show to friends,
- grocery lists you choose to share, preps you choose to share, and your likes, comments, "made it" marks and stars,
- your friends list, people you blocked, and reports you send.

Who sees what: preps you share with Friends are seen only by people you added as friends. Preps you share with
Everyone are seen by anyone signed in to Prepwise. A shared grocery list is seen only by people who have its code.

## Feedback
If you send feedback from the app, your note goes to the same database with the app version, phone model, iOS
version and a random id for this install (so repeated notes can be grouped), plus your name if you are signed in.
Only the developer can read it.

## AI features
Logging food by voice or photo, recipe search, import and grocery help use Claude. There are two ways it can run:

- **Prepwise's Claude (signed in, no key).** Your request, any photo you pick, and your food preferences (goals,
  macros, allergies, likes and rules) go through Prepwise's server to Anthropic. The server passes them on and keeps
  only a count of how many requests you made today, to enforce a fair daily limit. Anthropic handles the request
  under its commercial terms, which do not allow training on it.
- **Your own key.** If you save your own Anthropic or OpenAI key (kept in your phone's Keychain), the same
  information goes directly from your phone to that provider under your account, and Prepwise sees none of it.

Signing in or saving a key is how you agree to this; signing out or removing the key stops it.

**Logging food by voice, photo or Siri.** When you log by voice, the short recording goes through Prepwise's server
to a speech to text service (the Whisper model, run by Groq) and comes back as words. If you are not signed in or are
offline, Apple's speech recognition is used instead (on your phone when it supports that, otherwise through Apple).
With Siri, Siri hears you and hands Prepwise the words. Those words, or the photo you take of a meal, are sent to
Claude as described above so it can work out which foods and how much. To help spell and match your own food, the
names of your recipes, saved foods and recently logged foods go along with the recording and the words. Prepwise's
server does not keep the recording, the words, the photo or the answer; it keeps only a count of how many requests you
made today. The foods are then saved in your diary on your phone.

## Cook mode voice
When cook mode reads steps aloud with the natural voice, the text of each step goes through Prepwise's server to a
text to speech service (run by Groq) and comes back as audio. The audio is kept on your phone so each step is only
fetched once. Nothing about you goes with it. You can turn the natural voice off in Settings; the phone's own voice is
used instead and nothing leaves the phone. Hands-free commands in cook mode ("next", "back") use Apple's speech
recognition (on your phone when it supports that, otherwise through Apple).

## Reports and moderation
Reports you send are read by the developer, who removes content and people that break the community guidelines.

## Nutrition and barcodes
Food and ingredient names are sent to the USDA FoodData Central database to look up nutrition. Those lookups go
through Prepwise's server, which keeps the database's answer so the same food is not fetched twice. It does not record
who asked. If you are not signed in, it keeps a scrambled form of your network address for up to a day, only to cap
how many lookups one address can make in an hour. If you add your own USDA key, lookups go straight from your phone to
USDA instead. Scanned barcodes, and the words you type into food search, are also looked up on Open Food Facts,
straight from your phone. None of these lookups includes anything else about you.

## Apple Health
Everything here is optional and off until you turn it on.

- **Writing.** Prepwise can write the food you log (calories, protein, carbs, fat and other nutrients) to Apple Health.
- **Reading.** To adjust your daily targets, Prepwise can read the active calories you burn, your workouts and your
  body weight from Apple Health.

What it reads is used on your phone to work out your targets. It is never sent to Prepwise's server, to Claude, or to
anyone else, and it is never used for advertising.

## No tracking, no ads
Prepwise has no ads, no analytics SDKs, and does not track you across apps or websites. Nothing is sold.

## Deleting your data
Settings, Account, Delete my account removes everything Prepwise stored about you on the server: profile, friends,
shared preps, comments, likes, made it marks, reports and shared lists. Deleting the app removes everything on the
phone.

## Contact
Questions: christopherdunn321@gmail.com
