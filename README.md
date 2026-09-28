# AttendIQ — Phase 2

Premium Phase 2 extension of AttendIQ, built around the supplied 10 timetable PDFs.

## Includes
- Phase 1 attendance calculator and timetable-derived forecasting
- Visual attendance health dashboard
- Subject intelligence view
- Projected semester trajectory chart
- OD / Medical Leave simulator
- Ordinary absence simulator
- Timetable-aware affected-class calculation
- Irreversible Detention warnings
- Natural-language Attendance Advisor (runs locally in the browser)
- Dark/light premium UI
- Responsive desktop/tablet/mobile layout

## Run
```bash
npm install
npm run dev
```
Then open the Vite local URL, normally http://localhost:5173.

## Build
```bash
npm run build
```

## Data note
The project uses `src/data.json`, generated from the supplied timetable PDFs. The source PDFs are retained in `source-timetables/` for traceability. The challenge semester window is fixed to 29 Aug 2026 through 29 Nov 2026.

## OD / Medical simulation assumption
The simulator treats OD/Medical mode as eligible classes excluded from the attendance denominator. This is a modeling assumption for the demo; institutional attendance policy should be confirmed before real use.
