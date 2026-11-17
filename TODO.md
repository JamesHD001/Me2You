# Me2You Project TODO

This checklist tracks the work required to plan, design, build, test, and launch **Me2You: Your Communication Companion** across web, Android, and iOS.

Keep this file synchronized with `Me2You-documentation.txt`. Record unresolved decisions as pending rather than treating proposals as approved.

## 1. Product discovery and validation
- [ ] Research existing communication-development products and identify their strengths, weaknesses, and gaps.
- [ ] Interview target users about communication challenges and desired outcomes.
- [ ] Define primary user personas and priority use cases.
- [ ] Validate the four product pillars: Learn, Practise, Connect, Grow.
- [ ] Validate the curriculum stages and skill areas.
- [ ] Define measurable, privacy-conscious product success metrics.
- [ ] Conduct product-name, trademark, and domain checks for Me2You.

## 2. Product requirements and experience
- [ ] Define the MVP scope and release phases.
- [ ] Map key user journeys for web, Android, and iOS.
- [ ] Design onboarding and goal selection.
- [ ] Design the initial communication self-assessment.
- [ ] Define learning paths, lesson formats, and completion rules.
- [ ] Define AI practice exercises and feedback standards.
- [ ] Design post-session reflection and personal progress tracking.
- [ ] Define accessibility and low-bandwidth requirements.
- [ ] Create wireframes and a cross-platform design system.

## 3. Architecture and technology decisions
- [ ] Approve the cross-platform architecture.
- [ ] Evaluate Next.js/React/TypeScript for web.
- [ ] Evaluate React Native/Expo/TypeScript for Android and iOS.
- [ ] Decide on monorepo tooling and shared package boundaries.
- [ ] Evaluate Supabase/PostgreSQL against alternatives.
- [ ] Evaluate LiveKit Cloud and alternative video providers.
- [ ] Decide web hosting and backend deployment approach.
- [ ] Define development, staging, and production environments.
- [ ] Define CI/CD, code review, dependency management, and release workflows.
- [ ] Create architecture diagrams and an initial threat model.

## 4. Accounts, profiles, and verification
- [ ] Define registration, sign-in, recovery, and contact-verification flows.
- [ ] Define username rules, uniqueness, and username-change policy.
- [ ] Design public profiles and private account data separation.
- [ ] Define profile privacy and visibility controls.
- [ ] Decide what the verified badge actually verifies.
- [ ] Evaluate identity-verification methods and providers.
- [ ] Define verification review, expiration, appeal, and revocation workflows.
- [ ] Ensure verification status can only be changed by trusted server-side processes.
- [ ] Define account restriction and suspension states.

## 5. Learning and AI practice
- [ ] Build the initial communication curriculum.
- [ ] Write and review initial lessons and practical exercises.
- [ ] Define assessment criteria and personal progress indicators.
- [ ] Decide whether AI practice belongs in the first release.
- [ ] Select AI provider(s) and define a provider-independent service layer.
- [ ] Define AI privacy, retention, cost, usage, and safety controls.
- [ ] Test AI feedback for accuracy, usefulness, fairness, and tone.

## 6. Human conversations and matchmaking
- [ ] Define guided conversation missions and prompts.
- [ ] Define free conversation workflows and community boundaries.
- [ ] Design automatic matchmaking.
- [ ] Design user-selected/browse matchmaking.
- [ ] Define matching preferences and privacy-safe eligibility rules.
- [ ] Validate fixed session durations and flexible session limits.
- [ ] Implement private two-person video sessions only.
- [ ] Enforce the two-participant maximum on the server/provider side.
- [ ] Implement short-lived server-generated video access tokens.
- [ ] Implement consent before joining and clear session termination.
- [ ] Implement camera, microphone, connection, and error states.
- [ ] Implement block, report, and post-session reflection workflows.
- [ ] Test reconnect, poor-network, and session-cleanup behaviour.

## 7. Screen privacy and capture protection
- [ ] Document Android FLAG_SECURE support and limitations.
- [ ] Prototype and test Android protected-window behaviour on real devices.
- [ ] Document iOS scene-capture-state APIs and supported OS versions.
- [ ] Prototype iOS capture detection and sensitive-content response.
- [ ] Define platform-specific capture responses: warn, obscure, pause, or end.
- [ ] Account for legitimate accessibility and screen-mirroring scenarios.
- [ ] Define the web privacy notice and best-effort deterrents.
- [ ] Design and evaluate dynamic call watermarking.
- [ ] Clearly communicate that external-camera recording cannot be prevented.
- [ ] Ensure product messaging never promises absolute screenshot or recording prevention.

## 8. Safety, moderation, and age policy
- [ ] Decide the minimum age and age-assurance approach.
- [ ] Define safeguarding requirements before enabling matchmaking.
- [ ] Write community guidelines and prohibited-conduct rules.
- [ ] Design user reporting and moderation review workflows.
- [ ] Define urgent safety escalation and incident response.
- [ ] Define account restriction, suspension, and appeal processes.
- [ ] Evaluate abuse prevention, rate limits, and repeat-offender controls.
- [ ] Define moderator permissions and audit logging.

## 9. Privacy and security
- [ ] Map personal data and define data minimization.
- [ ] Define retention, export, and deletion policies.
- [ ] Draft privacy policy and terms of service.
- [ ] Review Nigeria Data Protection Act 2023 and other applicable regional requirements.
- [ ] Design database access controls and Row Level Security policies.
- [ ] Ensure roles, verification status, and permissions cannot be self-assigned by clients.
- [ ] Secure secrets and environment variables.
- [ ] Define administrator MFA and privileged-access controls.
- [ ] Apply an OWASP ASVS-informed security checklist.
- [ ] Plan backups, restoration tests, monitoring, and incident response.
- [ ] Review third-party provider data-processing and privacy terms.

## 10. Implementation and quality assurance
- [ ] Finalize repository structure for web, mobile, shared packages, backend, and tests.
- [ ] Create README.md, AGENTS.md, and .env.example.
- [ ] Establish formatting, linting, type-checking, and testing standards.
- [ ] Implement authentication and profile foundations.
- [ ] Implement learning and progress foundations.
- [ ] Implement AI practice if approved for the release.
- [ ] Implement video and matchmaking after safety readiness.
- [ ] Implement moderation and privacy controls.
- [ ] Add automated unit, integration, and end-to-end tests.
- [ ] Test web, Android, and iOS on supported devices and OS versions.
- [ ] Perform accessibility, performance, and security testing.
- [ ] Prepare release, support, and rollback procedures.

## 11. Launch readiness
- [ ] Complete user acceptance testing.
- [ ] Complete privacy, security, and safeguarding reviews.
- [ ] Confirm support and moderation capacity.
- [ ] Prepare help content and user education.
- [ ] Prepare web deployment and mobile store submissions.
- [ ] Monitor reliability, safety, user feedback, and product outcomes after launch.

## 12. Decisions awaiting approval
- [ ] Minimum age and age policy.
- [ ] Final web and mobile framework choices.
- [ ] Backend and database provider.
- [ ] Video infrastructure provider.
- [ ] AI provider and whether AI is in the MVP.
- [ ] Identity-verification method and badge meaning.
- [ ] Capture-detection response for each platform.
- [ ] Final session duration presets and flexible-session limits.
- [ ] MVP feature boundary and release sequence.
- [ ] Visual identity, design system, and brand clearance.

## Working rule
When a requirement or feature is added or changed:
1. Update `Me2You-documentation.txt` first.
2. Update this `TODO.md` second.
3. Keep confirmed decisions separate from proposals and open questions.
