# PULSE
My first mobile app — work in progress


<p align="center">
  <h1 align="center">PULSE</h1>
  <p align="center">All-in-one fitness tracking app — strength, WODs, Hyrox, combat & nutrition.</p>
  <p align="center">
    <img src="https://img.shields.io/badge/React_Native-0.81-blue?logo=react" alt="React Native" />
    <img src="https://img.shields.io/badge/Expo-54-000020?logo=expo" alt="Expo" />
    <img src="https://img.shields.io/badge/TypeScript-5.3-3178C6?logo=typescript" alt="TypeScript" />
    <img src="https://img.shields.io/badge/Supabase-Backend-3FCF8E?logo=supabase" alt="Supabase" />
    <img src="https://img.shields.io/badge/Status-In_Development-yellow" alt="Status" />
  </p>
</p>

> **My first mobile app — still in active development.**

## Demo

[![Watch the demo](https://img.shields.io/badge/Watch_Demo-YouTube-red?logo=youtube)](https://youtube.com/shorts/8kc1ykGCFvs?feature=share)

---

## About

Most fitness apps do one thing well — Pulse does everything. Built out of frustration with switching between 3+ apps to track workouts, nutrition and combat training.

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Framework | React Native + Expo (managed) |
| Language | TypeScript |
| Navigation | Expo Router (file-based) |
| Backend | Supabase (PostgreSQL + Auth + RLS) |
| State | Zustand |
| Animations | React Native Reanimated |
| Health | Apple HealthKit |
| Nutrition APIs | Open Food Facts, FatSecret |

## Features

**Workout Tracking**
- Strength training logger (sets, reps, weight, RPE)
- Rest timer with haptic feedback
- Automatic volume calculation
- Workout history with detailed breakdowns

**Training Modes**
- **Strength** — classic weightlifting
- **AMRAP / EMOM / For Time / Tabata** — CrossFit-style WODs
- **Hyrox** — full 16-station simulation
- **Combat Rounds** — boxing, MMA, Muay Thai presets

**Smart Features**
- Automatic **PR detection** with animated toasts
- **Progression suggestions** based on workout history
- **Plateau detection** + tips to break through
- **PR predictions** based on trends
- **Program generator** via questionnaire

**Nutrition**
- Calorie & macro tracker
- **Barcode scanner** (Open Food Facts + FatSecret)
- **Recipe suggestions** based on remaining macros

**Health**
- Apple HealthKit integration (steps, calories, distance)
- 210+ exercises (140 strength + 70 combat)
- Workout templates system

## Architecture

```
pulse/
├── app/                    # Screens (Expo Router)
│   ├── (auth)/             # Login, Register, Welcome
│   ├── (tabs)/             # Home, Train, Nutrition, Exercises, History, Profile
│   ├── workout/            # Active workout, WOD, Hyrox, Combat
│   └── nutrition/          # Barcode scanner
├── src/
│   ├── services/           # Business logic & API calls
│   ├── stores/             # Zustand state management
│   ├── types/              # TypeScript types
│   └── lib/                # Supabase client
└── docs/                   # SQL schemas & seeds
```

## License

This project is for personal/educational use.

