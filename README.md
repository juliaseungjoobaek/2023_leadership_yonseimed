# Promotion Requirement Calculator – Group 2 (Yonsei Med '23 Leadership Project)

🏆 **Grand Prize Winner**

A web-based tool to automatically check promotion eligibility and minor completion status for Yonsei College of Medicine students.

---

## Features

- Automated promotion requirement analysis  
- Supports both completed and planned course inputs  
- Minor progress tracking with smart recognition logic  
- Console-based detailed requirement breakdown  

---

## How to Use

### ✅ Input Completed Courses

1. Go to: Yonsei Portal → Academic Info → Grades → Full Transcript → Print → Save
2. Copy all text from the saved file and paste into the input field.

---

### 📝 Input Planned Courses

**Format:**
CourseCode,Type,Credits,Grade,AdditionalInfo(optional)

**Example:**
UCI1175,-,1,P,(연정인) AIC2130,대교,,C- BIO1102,대교,3,C+,어바 STA2102,,,B-

- `Type` and `Credits` are optional (auto-detection enabled but not always accurate)
- Valid Types: `일반`, `전기`, `전선`, `전필`, `교직`, `대교`, `교기`, `RC`, `-`, `UICE`, `MB`, `ME`, `CC`, `MR`, `LHP`
- Valid Grades: `A+`, `A0`, `A-`, `B+`, `B0`, `B-`, `C+`, `C0`, `C-`, `D+`, `D0`, `D-`, `F`, `P`, `NP`

---

## Notes

- Humanities in Medicine 3, 4 → Use `MED2111`, `MED2112`
- Courses like `STA1001` may be dual-counted (e.g., 필수교양 + 분야)
- Course data is stored via cookies
- Console (F12 → Console tab) shows detailed progress tracking

---

## Troubleshooting

- If transcript is unreadable, ensure:
  - You followed: `Full Transcript → Print → Save`
  - No "text as image" setting is enabled in your PDF viewer

- For misclassified planned courses (e.g., `AIC2130` as 대교 instead of 전선), manually specify:
AIC2130,전선,,C-


---

## Update Log (2023)

- **Sep–Oct**: GitHub launch, transcript parser, minor requirement logic
- **Oct 22–27**: UI/UX overhaul, admin tools, console info, bug fixes
- **Nov 1–22**: Expanded liberal arts info, crawler integration, public release
