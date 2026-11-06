finhealth/
├── backend/
│   ├── app/
│   │   ├── config.py                 # Settings & CORS config
│   │   ├── main.py                   # FastAPI app & endpoints
│   │   ├── models/
│   │   │   └── schemas.py            # Pydantic v2 data models
│   │   ├── parsers/
│   │   │   ├── base.py               # Normalization & column inference
│   │   │   ├── csv_parser.py         # Multi-bank CSV parser
│   │   │   ├── excel_parser.py       # Excel (.xlsx/.xls) parser
│   │   │   └── pdf_parser.py         # pdfplumber table & regex parser
│   │   ├── services/
│   │   │   ├── analytics.py          # Cashflow & recurring subscriptions
│   │   │   ├── anomaly.py            # IsolationForest & IQR anomaly engine
│   │   │   ├── categorizer.py        # Rules + ML fallback classifier
│   │   │   ├── recommender.py        # Smart actionable advice engine
│   │   │   ├── sample_generator.py   # Realistic 6-month statement generator
│   │   │   └── scoring.py            # 5-Pillar Financial Health Score
│   │   └── utils/
│   │       └── privacy.py            # Account & PII masking
│   ├── tests/
│   │   ├── conftest.py               # Pytest path configuration
│   │   ├── test_api.py               # Integration tests
│   │   ├── test_categorizer.py       # Taxonomy tests
│   │   ├── test_parsers.py           # Parsing & masking tests
│   │   └── test_scoring.py           # Health score unit tests
│   ├── requirements.txt              # Python dependencies
│   └── .env.example
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── AnomalyAlerts.jsx     # Outlier alerts
│   │   │   ├── CashflowTrendChart.jsx# Monthly inflow vs outflow Recharts
│   │   │   ├── CategoryBreakdown.jsx # Donut & ranked spending list
│   │   │   ├── HealthScoreGauge.jsx  # Radial gauge & formula modal
│   │   │   ├── HeroUpload.jsx        # Drag-and-drop file uploader
│   │   │   ├── Navbar.jsx            # Header, theme, & currency toggle
│   │   │   ├── Recommendations.jsx   # Actionable financial advice
│   │   │   ├── RecurringPayments.jsx # Detected subscriptions
│   │   │   ├── ReportModal.jsx       # Printable executive report
│   │   │   ├── SummaryCards.jsx      # KPI summary cards
│   │   │   └── TransactionsTable.jsx # Searchable & filterable ledger
│   │   ├── context/
│   │   │   └── ThemeContext.jsx      # Dark/light theme provider
│   │   ├── services/
│   │   │   └── api.js                # API client with XHR progress
│   │   ├── App.jsx                   # Root application state
│   │   ├── index.css                 # Tailwind & print styles
│   │   └── main.jsx
│   ├── index.html
│   ├── package.json
│   ├── tailwind.config.js
│   ├── vite.config.js
│   └── .env.example
├── sample_data/
│   ├── sample_bank_statement.csv     # Ready-to-upload sample statement
│   └── sample_bank_statement.xlsx    # Excel format test statement
├── DEPLOYMENT.md                     # Step-by-step deployment guide
├── LICENSE                           # MIT License
└── README.md
```
