# Yunlong (Adler) Lu

Stevens Institute of Technology, B.S. Computer Science, expected May 2028; looking for Summer 2027 software engineering internships. Based between Hoboken, NJ and Los Angeles.

## Projects

- **[pgqueue](https://github.com/adleraaa/pgqueue)**: durable job queue on a single PostgreSQL table, with a FastAPI API for producers and a Python worker library. Workers claim jobs with `SELECT ... FOR UPDATE SKIP LOCKED` and a lease kept alive by a heartbeat; failed jobs retry with exponential backoff and are dead-lettered after `max_attempts`.
- **[hudson-transit](https://github.com/adleraaa/hudson-transit)**: live arrivals board for PATH and the NYC Subway (Next.js, TypeScript). Normalizes PATH's JSON feed and the MTA's eight GTFS-realtime feeds into one zod-validated schema. [Live](https://hudson-transit.vercel.app)
- **[nyc311-pipeline](https://github.com/adleraaa/nyc311-pipeline)**: incremental ELT of NYC 311 service requests into DuckDB, modeled with dbt, with data-quality checks, refreshed daily by GitHub Actions. [Dashboard](https://adleraaa.github.io/nyc311-pipeline/)
- **[toolcall-qlora-bfcl](https://github.com/adleraaa/toolcall-qlora-bfcl)**: QLoRA fine-tune of Qwen2.5-1.5B-Instruct for function calling on one 8 GiB laptop GPU, measured on Berkeley Function Calling Leaderboard (BFCL) tasks, including how much it hurt the model's ability to decline when no function fits.
- **[offerpilot](https://github.com/adleraaa/offerpilot)**: local, human-in-the-loop job-search pipeline. Pulls postings from public ATS APIs, drops ones that break hard constraints with deterministic rules, scores the rest with one LLM call, and stops at a SQLite review queue. Nothing is sent to employers.
- **[internradar-ai](https://github.com/adleraaa/internradar-ai)**: internship tracker for undergraduate CS students. Candidate postings come from the SimplifyJobs list; each kept entry links to the official application page and carries a last-verified date. A GitHub Actions job updates the list daily. [Live](https://internradar-ai.vercel.app)

## Contact

- Email: adler1433223@gmail.com
- LinkedIn: [yunlong-lu](https://www.linkedin.com/in/yunlong-lu-0964bb389)
