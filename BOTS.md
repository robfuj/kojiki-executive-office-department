# Bots of Executive Office / Chief of Staff  (docx S5 candidate menu)

These are the **Major sub-functions** of Executive Office / Chief of Staff from the spec. Each is a bot — a
child decision system that can be instantiated to do the actual work.

## Install flow (matches the Orientation Protocol)
1. **Orient** — the agent runs the Kojiki Orientation Protocol (name / industry /
   jurisdiction / siblings).
2. **Research** — the agent researches the field and decides which sub-functions this
   specific org needs.
3. **Install** — instantiate only the chosen bots:
   ```bash
   cd bots
   python3 install_bots.py brand growth performance-marketing
   ```
   (use the slugs listed below; omit args to install all). Each installed bot becomes a
   full decision system under `bots/<slug>/` with README + AGENT.md + schemas + a stub
   decision record, and registers under this department's group_id for handoffs.

Total candidates: 7.

- `executive-priorities` — **Executive Priorities**  ·  titles: Chief of Staff, Deputy Chief of Staff, Executive Director, Strategic Projects Lead, Executive Operations Manager
- `decision-management` — **Decision Management**  ·  titles: Chief of Staff, Deputy Chief of Staff, Executive Director, Strategic Projects Lead, Executive Operations Manager
- `cross-functional-coordination` — **Cross-Functional Coordination**  ·  titles: Chief of Staff, Deputy Chief of Staff, Executive Director, Strategic Projects Lead, Executive Operations Manager
- `strategic-initiatives` — **Strategic Initiatives**  ·  titles: Chief of Staff, Deputy Chief of Staff, Executive Director, Strategic Projects Lead, Executive Operations Manager
- `executive-intelligence` — **Executive Intelligence**  ·  titles: Chief of Staff, Deputy Chief of Staff, Executive Director, Strategic Projects Lead, Executive Operations Manager
- `decision-cadence` — **Decision Cadence**  ·  titles: Chief of Staff, Deputy Chief of Staff, Executive Director, Strategic Projects Lead, Executive Operations Manager
- `follow-through` — **Follow-through**  ·  titles: Chief of Staff, Deputy Chief of Staff, Executive Director, Strategic Projects Lead, Executive Operations Manager
