# navafit
hindufitness app

NavaFit is a cutting-edge wellness super app that combines fitness tracking, AI-powered nutrition analysis, intelligent coaching, and mindfulness practices into a seamless, glassmorphic SwiftUI experience. Built for 2025 with the latest iOS technologies and AI/ML capabilities.

### 🎯 Core Features
**Project structure to be modular, scalable, and AI/ML-driven.With Swarm/Hive Mind agent workflows for multi-agent development.**

- **🏋️ Akhada**: Advanced workouts and tracking with HealthKit integration
- **🍎 Mitahara**: AI-powered nutrition analysis and meal planning
- **🧠 Guru**: Intelligent AI coach with voice interaction , Location Ans weatherkit Intergration (Singapore)
- **📊 Dashboard**: Comprehensive health metrics visualization, Daily Baghavad Gita Quotes. Profile.
- **⚙️ Settings**: User preferences and data management, Social Media Connections.

## 🏗️ Architecture

### Technology Stack

- **Frontend**: SwiftUI with glassmorphic design system, Dark Lineargradient background, Dark Blue Accent And Glowing Blue Minimalist Icons.
- **Backend**: Firebase (Auth, Firestore, Storage, Analytics)
- **AI/ML**: Core ML models + OpenAI/Claude API integration
- **Health**: HealthKit for comprehensive health data
- **Voice**: ElevenLabs TTS + Apple Speech Recognition
- **Analytics**: Firebase Analytics + custom event tracking
- **Monetization**: StoreKit 2 for premium features

### Project Structure & Folders/Files Layout 

```
NavaFit/
├── .claude/                    # Claude Code AI agents configuration
│   ├── agents/                 # Specialized AI development agents
│   └── settings.json           # Claude Flow configuration
├── AIEngine/                   # AI/ML services and models
│   ├── Agents/                 # AI agent configurations
│   ├── MLModels/               # Core ML models and loaders
│   └── Services/               # AI service implementations
├── App/                        # Core app configuration
├── Models/                     # Data models and schemas
├── Services/                   # Business logic services
│   ├── Firebase/               # Firebase integration
│   ├── Health/                 # HealthKit services
│   ├── Analytics/              # Advanced analytics
│   └── Monetization/           # Premium features and subscriptions
├── UI/                         # User interface components
│   ├── Components/             # Reusable UI components
│   ├── Views/                  # App screens and views
│   └── Animations/             # Lottie and custom animations
├── Tests/                      # Comprehensive test suite
│   ├── Unit/                   # Unit tests
│   ├── Integration/            # Integration tests
│   └── UI/                     # UI automation tests
└── Resources/                  # Assets, fonts, and configurations

- **App/**
  - `NavaFitApp.swift`: Main SwiftUI entry point
  - `AppDelegate.swift`: Firebase/Push config
  - `Theme.swift`: Colors, gradients, glass, fonts
  - `ThemeManager.swift` : Dynamic theme switching
  - `Constants.swift`: Global constants, API keys
  - `Config.swift` : Non-secret env, locales, build flags
  - `AppViewModel.swift` : Global app state, onboarding, deep links
  - `DeepLinkHandler.swift` : Universal links, QR codes

- **Onboarding/** 
  - `OnboardingView.swift`: User onboarding flow
  - `PermissionsManager.swift`: HealthKit, Notifications, Location permissions

- **AIEngine/**
  - `AIManager.swift`: Claude/OpenAI/Vertex queries
  - `FirebaseAIService.swift`: AI via Firebase/Firestore triggers
  - `AIDataParser.swift`: Parse/structure AI responses
  - `AIPromptLibrary.swift` : Versioned, updatable prompts/templates
  - `SpeechService.swift` : TTS/STT (ElevenLabs, Apple, etc)
  - **Agents/** 
    - `AgentConfig.yaml` : Multi-agent config for Claude Flow
  - **MLModels/**
    - `ActivityClassifier.mlmodel`
    - `NutritionPredictor.mlmodel`
    - `ModelLoader.swift`

- **Services/**
  - `FirebaseService.swift`: DB, listeners, writes
  - `AuthService.swift`: Sign-in with Apple/Google/Email
  - `UserService.swift`: Profile CRUD
  - `CollectiveService.swift`: Groups, feed, posts, chat
  - `SyncService.swift`: HealthKit, iCloud sync
  - `WeatherService.swift`: WeatherKit
  - `NotificationService.swift` : Push/local, reminders
  - `AnalyticsService.swift` : Firebase Analytics, custom events
  - `RemoteConfigService.swift` : Firebase RemoteConfig/feature flags
  - `BadgeService.swift` : Gamification (badges, leaderboards)
  - `PurchaseService.swift` : StoreKit 2 / In-App Purchase/Subscription
  - `ReportContentService.swift` : Report/block users (community safety)
  - `CrashReportingService.swift` : Crashlytics/Sentry integration

- **Models/**
  - `UserModel.swift`
  - `WorkoutModel.swift`
  - `NutritionModel.swift`
  - `CoachResponse.swift`
  - `CollectiveModel.swift`
  - `UIStateModel.swift`
  - `AchievementModel.swift` 
  - `BadgeModel.swift` 
  - `PurchaseModel.swift` 

- **UI/**
  - **Components/**
    - `GlassTabBar.swift`
    - `GlowingIcon.swift`
    - `GlassTileCard.swift`
    - `VerticalCarouselView.swift`
    - `AnimatedBackground.swift`
    - `PaywallView.swift` 
    - `FeatureTile.swift`
  - **Views/**
    - `DashboardView.swift`
    - `AkhadaView.swift`
    - `AIDenView.swift`
    - `CollectivesView.swift`
    - `ProfileView.swift`
    - `SettingsView.swift` 
  - **Animations/**
    - `WarriorViewTransition.swift`
    - `SmoothListAnimation.swift`
    - `LoadingShimmer.swift`

- **Extensions/**
  - `UIColor+Extensions.swift`
  - `View+Animations.swift`
  - `UIFont+NavaFit.swift`
  - `Image+Glow.swift`
  - `ViewModifiers.swift`

- **Utilities/**
  - `HapticEngine.swift`
  - `GlitchGlareEffect.swift`
  - `CarouselScroller.swift`
  - `Debouncer.swift`
  - `Accessibility.swift` 

- **Resources/**
  - `Assets.xcassets/`
  - **Fonts/**
    - `PlayfairDisplay-VariableFont_wght.ttf`
    - `PlayfairDisplay-Italic-VariableFont_wght.ttf`
  - **LottieAnimations/**
  - **Localizations/**

- **Tests/**
  - `AIEngineTests.swift`
  - `ViewModelTests.swift`
  - `UIInteractionTests.swift`

- **Packages/**
  - Firebase (SPM)
  - SwiftUIX
  - Lottie
  - CombineExt
  - Kingfisher
  - SwiftCharts

- **Prompts/**
  - `NavaFit_Instructions.md`
  - **FeaturePrompts/**
    - `AIEngine.md`
    - `UI.md`

- **Docs/** 
  - `README.md`

- `TASKS.md`: Task manager file

```

## 🚀 Getting Started

### Prerequisites (Claude Code to check, Before starting and install missing Package Dependencies)

- Xcode 16.4+ (iphone 15 pro max simulator ios 17.0)
- iOS 17.0+
- SwiftUIX
- Firebase project connection established with all neccessary dependencies. just double check .
- HealthKit/WeatherKit/Apple Sign In 
- Lottie 4.5.2
- CombineExt
- SwiftCharts
- Glassmorphism-UI Repository
- Google Sign-in 9.0.0

**For Cursor Extensions:**

- Enable/Install (via Cursor > Extensions panel):
  - `Claude Code` (opus)
  - `Claude Flow` (multi-agent)
  - `SPM` (Swift Package Manager UI)
  - `Claude Code Sub Agents` ([see GitHub](https://github.com/claude-code-sub-agents))

### 3️⃣ Configure Claude Agents and Prompts

- Add/update `.claude/agents/` with at least:
  - `ui-designer.md`: SwiftUI, glassmorphic, Playfair font UI design
  - `firebase-handler.md`: Firebase, Firestore, auth, storage config
  - `ml-specialist.md`: AI/ML model integration (vision, nutrition, classifier)
  - `security-reviewer.md`: App security, best practices, review
- Link relevant `/Prompts/FeaturePrompts/*.md` for context engineering

---

### Installation

2. **Install dependencies**
   ```bash
   # Swift Package Manager will resolve dependencies automatically
   # when you open the project in Xcode
   open NavaFit.xcodeproj
   ```

3. **Configure Firebase**
   - Add your `GoogleService-Info.plist` to the project
   - Enable Authentication, Firestore, Storage, and Analytics
   - Set up security rules for Firestore

4. **Configure API Keys**
   ```bash
   # Create environment configuration
   cp .env.example .env
   # Add your API keys (OpenAI, ElevenLabs, etc.)
   ```

5. **Enable Capabilities**
   - WeatherKit
   - HealthKit
   - Push Notifications
   - Background App Refresh
   - In-App Purchase
   - Sign In With Apple
   
### Automated Clean, Test, and Build Instructions (Strictly Do This Befor Moving On To Next Task. Ensure All Folders & Files Are Correct)

- After creating files/folders and updating packages:
  - Run: **Xcode > Product > Clean Build Folder**
  - Then: **Product > Build & Run**
  - In Cursor: Use **Test Runner** (if enabled), and run `/Tests/*` files.
- Report and pause on **any error, conflict, or missing dependency**.
  - **Do not auto-fix—first explain the cause, proposed fix, and ask for my approval to proceed.**

### Development Setup

#### Using Claude Code + Claude Flow (Recommended)

1. **Install Claude Code**
   ```bash
   npm install -g @anthropic-ai/claude-code
   ```

2. **Add Claude Flow MCP Server**
   ```bash
   claude mcp add claude-flow npx claude-flow@alpha mcp start
   ```

3. **Initialize Development Swarm**
   ```bash
   npx claude-flow@alpha swarm init --topology hierarchical --agents 8
   ```

4. **Start Multi-Agent Development**
   - UI Designer: SwiftUI components and glassmorphic design
   - Firebase Handler: Backend services and data management
   - ML Specialist: AI/ML models and Core ML integration
   - Security Reviewer: Privacy compliance and security audits

## 🎨 Design System

### Visual Identity

- **Primary Colors**: (#2D9DFF light / #000507 dark)
- **Secondary Colors**: (#280ED6 light / #02080A dark)
- **Background**: Glassmorphic UI blur effects with subtle gradients
- **Typography**: Playfair Display (elegant serif) + SF Pro (system)
- **Icons**: Minimalist Glowing Neon Blue Icons/Logos
- **Navigation**: 5 Tab Bottom Navigation Bar
- **Animations**: Button Press Animations: (Visual feedback like color changes, scaling, or ripple effects when users tap.) Loading Indicators: (Engaging animations to reduce perceived wait times.)
Toggle Switches: (Smooth sliding animations that visually explain on/off states)
Pull to Refresh: (Animated cues signaling content refresh.)
Progress Bars: (Subtle animations reflecting progress in tasks or uploads.)
- **Transitions**:Morphing Elements: (Transforming buttons or icons into new components during navigation.)
Slide and Fade: ((Moving content in or out.)
Zoom Effects: (Bringing focus)

### Components
- No clutter Blending Functionality With Utilities
- Glass cards with blur effects and subtle borders
- Smooth animations and micro-interactions
- 5 Tab Bottom Navifation Bar
- Vertical Carousel with micro-interaction
- Clean Transitions No Delays 
- Contextual haptic feedback
- Voice interaction indicators
- Accessibility-first design

## 🤖 AI Features

### Core ML Models

- **Activity Classifier**: Automatic workout detection from sensor data/Search Web For Recommended Workout Programme Based On Age,Fitnesslevel,Height/Weight Interests (Data Collected At Onboarding)
- **Nutrition Predictor**: Calorie and macro estimation from food images Based On Workout Programme
- **Health Trend Analyzer**: Pattern recognition in health metrics
- **Personalization Engine**: User preference learning and adaptation
- **Training**: Use Agent to generate Visual and Audio Learning for Macebell/Animal Flow/Yoga And BreathWork

### Voice Integration

- **ElevenLabs TTS**: Premium text-to-speech for AI coach
- **Apple Speech**: System fallback and voice input recognition
- **Natural Language Processing**: Contextual conversation understanding

### Books

- Basics On Gadah & Animal Movement Workouts
- Basic BreathWork & Yoga

## 🔒 Security & Privacy

### Data Protection

- **End-to-end encryption** for sensitive health data
- **Keychain storage** for API keys and tokens
- **Certificate pinning** for network security
- **Biometric authentication** (Face ID/Touch ID)

### Compliance

- **GDPR** compliant data handling
- **CCPA** privacy rights implementation
- **HIPAA** considerations for health data
- **App Store** privacy requirements

## 💰 Monetization

### Subscription Tiers

- **Free**: Basic tracking, limited AI interactions
- **Premium ($9.99/month)**: Unlimited AI coach, advanced analytics
- **Pro ($19.99/month)**: Nutrition scanning, social features, data export
- **Lifetime ($199.99)**: All features permanently

### Premium Features

- AI Personal Coach with voice interaction
- Advanced health analytics and insights
- Nutrition scanning and meal planning
- Social challenges and community features
- Data export and synchronization
- Priority customer support



## 📊 Analytics & Monitoring

### Key Metrics

- **User Engagement**: DAU/MAU, session duration, feature usage
- **Health Impact**: Goal achievements, behavior changes
- **Revenue**: Subscription conversion, retention rates
- **Technical**: App performance, crash rates, API latency

### Monitoring Stack

- **Firebase Analytics**: User behavior and custom events
- **Firebase Crashlytics**: Crash reporting and stability monitoring
- **Custom Analytics**: Health-specific metrics and insights
- **Performance Monitoring**: Real-time app performance tracking

## 🚀 Deployment

### Environments

- **Development**: Local development with Firebase emulators
- **Staging**: TestFlight beta testing with staging Firebase
- **Production**: App Store release with production Firebase

### CI/CD Pipeline

1. **Code Quality**: SwiftLint, unit tests, security scanning
2. **Build**: Xcode Cloud automated builds
3. **Testing**: Automated UI tests, integration tests
4. **Deploy**: TestFlight → App Store phased rollout

## 🤝 Contributing

### Development Workflow

1. **Feature Planning**: Use Claude agents for requirement analysis
2. **Implementation**: Multi-agent development with Claude Flow
3. **Testing**: Comprehensive test coverage with quality gates
4. **Review**: Security audit and code quality assessment
5. **Deployment**: Automated CI/CD pipeline

### Code Style

- Follow Apple's SwiftXUI style guide
- Use SwiftLint for consistent formatting
- Document public APIs with Swift DocC
- Maintain >80% test coverage

## 📚 Documentation

- [Architecture Guide](./Architecture.md)
- [API Documentation](./API.md)
- [Security Guidelines](./Security.md)
- [Deployment Guide](./Deployment.md)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](../LICENSE) file for details.

## 🙏 Acknowledgments

- **Firebase**: Backend infrastructure and analytics
- **OpenAI/Anthropic**: AI and language model capabilities
- **ElevenLabs**: Advanced text-to-speech technology
- **Lottie**: Smooth animations and micro-interactions
- **Community**: Open source contributors and beta testers

---

<div align="center">
  <p><strong>Built with ❤️ for the wellness community</strong></p>
  <p>NavaFit - Transforming lives through intelligent wellness technology</p>
</div>
