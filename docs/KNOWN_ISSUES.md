# Known Issues

The following issues were identified during the recent audit:

1. **Homepage Seminar-Room:** The live seminar-room claim on the homepage is not implemented.
2. **Research Studio Feedback:** Rule-based feedback in the Research Studio is occasionally mislabeled or ambiguous.
3. **Seminar Synthesis Payload:** Frontend/backend payload compatibility issues in the Gemini seminar synthesis (`synthesize.js`).
4. **Supabase Auth Restriction:** Email-domain restriction (`@saschina.org`) verification logic needs hardening/verification.
5. **RLS Verification:** Row Level Security rules on Supabase tables require thorough auditing.
6. **Progress Synchronization:** Sync verification needed for user progress saving.
