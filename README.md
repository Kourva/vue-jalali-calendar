<div align="center">
    <h1>Persian Calendar for Vue/Nuxt</h1>
    <p>A beautiful, theme-ready Jalali calendar component built with Vue 3.</p>
</div>

<br><br>

# ¶ A Message to You
I built this because every Persian calendar project I worked on needed the same fixes: RTL layout, Friday weekends, Jalali dates, event colors, and themes that don't break. or simply, It's not FREE!<br><br>
So here it is. Free. Open. Yours. **Not to be the best. Just to be useful.** Use it, break it, fix it, share it.

<br>

# ★ Features
+ 🌙 **Jalali Calendar**: Accurate Persian date conversion
+ 🎨 **114+ Premium Themes**: Netflix, Tiffany, Spotify, Iran, and 100+ more
+ 📱 **Fully Responsive**: Works on mobile, tablet, desktop
+ ⌨️ **Keyboard Shortcuts**: Navigate like a pro
+ 📅 **Event System**: Add events with categories & colors
+ 🔁 **Yearly Recurring**: Use *-1-1 for Nowruz every year
+ 🎯 **Today Highlight**: Never lose track
+ 📤 **Export Ready**: JSON, CSV, iCal support (coming soon)
+ ⚡ **Haptic Feedback**: Nothing Phone optimized
+ 🌍 **Dual Display**: See both **Jalali** & **Gregorian** calendars at a glance, no confusion, no conversion.

<br>

# ⌗ Quick Start
Just copy and paste the calendar folder anywher you want (e.g. src/components) and import calendar's style in your `main.js` or `nuxt config` or even inside the template per calendar use.

> [!WARNING]
> # Use ClientOnly in Nuxt
> Since the calendar uses browser APIs (like navigator and Intl), you need to wrap it inside `ClientOnly`:
> ```vue
> <template>
>     <ClientOnly>
>         <Calendar .../>
>     </ClientOnly>
> </template>
> ```

Example usage:
```vue
<template>
    <Calendar 
        v-model:year="year"
        v-model:month="month"
        v-model:day="day"
        :events="events"
    />
    <!-- And more props and emits -->
</template>

<script setup lang="ts">
import Calendar from 'path-to-calendar/Calendar.vue';
import 'path-to-calendar/assets/calendar.css';

const year = ref<number>(1403);
const month = ref<number>(7);
const day = ref<number>(20);
</script>
```

<br>

# ヅ One Component, Infinite Looks

```vue
<!-- Just change the data-theme attribute -->
<Calendar theme="netflix" />   <!-- Bold & dramatic -->
<Calendar theme="tiffany" />   <!-- Elegant & fresh -->
<Calendar theme="iran" />      <!-- Proud & premium -->
<Calendar theme="glass" />     <!-- Modern & sleek -->
```

114+ themes ready to use. Zero CSS conflicts. You can make your custom theme theme using the data-theme!

<br>

# Thank You

I've been working on this for a while because of the current situation in IRAN , and I know if i share this repo many of you will be waiting. Sorry for the delay — I wanted to make sure it was actually useful before sharing.

<br>

# License

**MIT** — Use it anywhere, no questions asked.

<br>

# Contributing

Found a bug? Have an idea? Open an issue or PR. Let's make this better together.

<br><br>

### Made with love for the Persian community and open source friends everywhere. Hope you find this helpful.
