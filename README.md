 IPL Analysis Dashboard (2008–2025)

A fully static, single-page IPL Analytics Dashboard built from raw ball-by-ball data covering all 18 IPL seasons from 2008 to 2025. No backend, no build step, no server just host the files and it works.

ipl-dashboard/
├── index.html                  
├── images/
│   ├── README.md               
│   ├── sai_sudharsan.jpg        
│   ├── prasidh_krishna.jpg     
│   └── nicholas_pooran.jpg      
├── ball_by_ball_data.csv       
├── ball_by_ball_data.csv.gz     
├── teams_data.csv               
├── .gitignore
└── README.md                    


🗂 Data Schema

ball_by_ball_data.csv (278,205 rows × 30 columns)

ColumnDescriptionseason_idIPL season year (2008–2025)match_idUnique match identifierbatterBatter's namebowlerBowler's nameteam_battingBatting teamteam_bowlingBowling teamover_numberOver (0-indexed)ball_numberBall within overbatter_runsRuns scored by batterextrasExtra runstotal_runsTotal runs on that ballis_wicketTRUE/FALSEwicket_kindHow out (bowled, caught, etc.)is_wide_ball / is_no_ball / is_leg_bye / is_bye / is_penaltyExtras flagsis_super_overTRUE/FALSEinnings1 or 2

teams_data.csv (16 rows × 4 columns)

ColumnDescriptionteam_idUnique team IDteam_nameFull team nameteam_name_short2–4 letter abbreviationimage_urlTeam logo URL


🛠 Tech Stack


HTML5 + CSS3 — Custom design system, zero frameworks
Vanilla JavaScript — All interactivity, no dependencies
Embedded base64 assets — Social icons, IPL/Tata logos, Orange/Purple Cap icons baked directly into index.html (no broken external links)
Real player photos — Loaded from local images/ folder
