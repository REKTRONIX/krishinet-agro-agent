# krishinet-agro-agent
Low-cost Model-Based RL Agent using Kalman Filter, Q-Learning and Markov Decision Process for small Indian Farmers - No Satellite needed
krishinet/
├── ARCHITECTURAL_DIAGRAMS.md          # Visual Block Diagram, Agent UML & Sequence Diagrams
├── README.md                          # Architecture, quickstart, sensor specs, & run guides
├── package.json                       # Dependencies & npm scripts
├── server.ts                          # Express backend with dual ports (8080/3000) & Gemini AI
├── vite.config.ts                     # Vite build & bundler configuration
├── tsconfig.json                      # TypeScript compiler configuration
├── index.html                         # Single-page application entrypoint
├── krishinet_agro_agent.R             # Statistical agro-agent simulation in R
├── metadata.json                      # Project metadata
├── .env.example                       # Environment template
├── .gitignore
├── bun.lock
├── scripts/
│   └── pack_krishinet.py              # Packaging script
├── src/
│   ├── main.tsx                       # React application bootstrap
│   ├── App.tsx                        # Dashboard layout & simulation orchestrator
│   ├── index.css                      # Tailwind styles & theme variables
│   ├── types.ts                       # TypeScript domain models and state interfaces
│   ├── context/
│   │   └── LanguageContext.tsx        # Multilingual state provider (HI, MR, PA, GU, EN)
│   ├── i18n/
│   │   └── translations.ts            # Localized agricultural dictionary
│   ├── components/
│   │   ├── Header.tsx                 # Telemetry badges, controls, & Codebase (.zip) download
│   │   ├── FiveSensorPanel.tsx        # Soil, microclimate, NPK, leaf wetness gauges
│   │   ├── KalmanFilterView.tsx       # Raw sensor vs EKF smoothed signals comparison
│   │   ├── QLearningMDPView.tsx       # Q-Matrix heatmap, policy explorer & state breakdown
│   │   ├── IndianHardwarePanel.tsx    # 3-Phase voltage, motor starter & drip manifolds
│   │   ├── LocalizedWeatherForecastWidget.tsx # 7-Day grounded agrometeorology
│   │   ├── CCTVFeed.tsx               # Live canopy camera & visual inspection
│   │   ├── GeminiAgronomistModal.tsx  # Multimodal AI agronomist chat & prescriptions
│   │   ├── StressSimulatorModal.tsx   # Heatwave, drought & grid disturbance injector
│   │   ├── ExportTelemetryModal.tsx   # CSV dataset exporter
│   │   ├── ZoneResourceEfficiencyHeatmap.tsx # Multi-zone water/fertilizer efficiency
│   │   ├── FertilizerScheduler.tsx    # Venturi fertigation recipe scheduler
│   │   ├── YieldAndClimateModel.tsx   # Yield prediction vs thermal/water stress
│   │   ├── MqttTrafficHourlyChart.tsx # MQTT edge broker traffic analytics
│   │   ├── LanguageSwitcher.tsx       # Language switcher component
│   │   └── ToastContainer.tsx         # Real-time event toast notifications
│   └── utils/
│       ├── kalman.ts                  # Extended Kalman Filter algorithm
│       ├── rlEngine.ts                # Q-Learning discrete MDP engine
│       ├── mockFarmData.ts            # Indian farm zones (Sugarcane, Cotton, Wheat, Mustard)
│       ├── mqttSimulator.ts           # Synthetic MQTT packet generator & jitter simulator
│       ├── fertilizerRecipes.ts       # Crop-specific NPK & micronutrient formulations
│       ├── pestKnowledge.ts           # Agronomic pest & disease knowledge base
│       ├── telemetryExport.ts         # CSV dataset generation utility
│       ├── audioAlerts.ts             # Speech synthesis & warning beeps
│       └── yieldRegression.ts         # Crop yield estimation equations
