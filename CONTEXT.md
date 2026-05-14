# IELTS Preparation - Context File

## Overview
This is an IELTS Band 6.5-7 preparation system with **MD-based practice** approach.

## Current Folder Structure

```
IELTS_Preparation/
├── CONTEXT.md                    # This file - system overview
├── progress.md                # Overall progress tracking (assistant updates)
├── dashboard.html            # Visual progress dashboard
├── quiz/                     # Practice files (user fills these)
│   ├── writing_task1/
│   │   ├── prompt1.md       # Bar Chart - Sports by Age
│   │   ├── prompt2.md       # Line Graph - Transport
│   │   ├── prompt3.md      # Pie Chart - Reasons for Study
│   │   ├── prompt4.md     # Process Diagram - Chocolate
│   │   └── prompt5.md    # Bar Chart - Student Enrollment
│   ├── writing_task2/
│   │   └── prompt1.md     # Discussion - University subjects
│   ├── listening/
│   │   └── prompt1.md    # Hotel conversation
│   ├── speaking/
│   │   └── cuecard1.md # Part 2 - Skill learned
│   └── reading/
│       └── passage1.md  # Reading practice
├── writing/                  # Writing guides + assessment
│   ├── guide.md           # Task 1 guide
│   ├── guide_task2.md    # Task 2 guide
│   └── assessment_log.md # Writing scores log
├── speaking/              # Speaking guides
│   ├── part1_guide.md
│   ├── part2_guide.md
│   └── part3_guide.md
├── listening/             # Listening guide
│   └── guide.md
├── grammar/              # Grammar materials
│   ├── guide.md
│   ├── exercises.md
│   └── basic.md
└── vocabulary/         # Vocabulary materials
    └── test.md
```

---

## How It Works

### Practice Flow
1. User practices by filling in MD quiz files in `quiz/` folder
2. User notifies assistant when a file is done
3. Assistant reads the file from `quiz/`, assesses the work
4. Assistant adds Band 6 & 9 example essays to the file
5. Assistant updates `progress.md` with score + date
6. Assistant updates `dashboard.html` practice log (categorized by skill)
7. Dashboard displays progress automatically

### Assessment Workflow (For Assistant)

When user says they're done with a practice file:

**Step 1:** Read the file from `quiz/` folder
- Determine skill type from folder name (writing_task1, writing_task2, listening, speaking, reading)

**Step 2:** Assess based on IELTS criteria
- Writing Task 1: Word count (150+), paraphrase, data accuracy, overview, comparison, linking words, paragraphs
- Writing Task 2: Word count (250+), opinion, examples, structure, linking words
- Speaking: Fluency, vocabulary, grammar, pronunciation
- Listening: Accuracy, spelling, numbers

**Step 3:** Score the work
- Band 5.0-5.5: Major issues (word count, grammar, structure)
- Band 6.0: Good but some issues
- Band 6.5+: Solid performance

**Step 4:** Add examples to the practice file
- Add Band 6 example (150-165 words for Task 1, 250-270 for Task 2)
- Add Band 9 example (170-190 words for Task 1, 280-300 for Task 2)
- Show the difference between bands

**Step 5:** Update progress.md
- Add entry to Practice Log table with: date, task, prompt, score, feedback
- Update Current Estimated Scores if improved

**Step 6:** Update dashboard.html
- Add entry to practiceLog object in the script
- Categorize by skill type: 'writing_task1', 'writing_task2', 'speaking', 'listening', 'reading', 'grammar', 'vocabulary'

**Step 7:** Provide feedback
- Give actionable next steps
- Focus on the biggest issues first

---

## Current User Profile

### Target
- **Band Goal**: 6.5 (Stretch: 7.0)
- **Timeline**: 1-2 months
- **Priority**: Writing Task 1 (word count) + Speaking (fluency)

### Current Estimated Scores
| Skill | Band | Notes |
|-------|------|-------|
| Reading | 6.5 | Good comprehension |
| Listening | 6.5 | Good understanding |
| Writing Task 1 | 5.0 | Issues: word count (~80-95), no paragraphs |
| Writing Task 2 | 6.0 | Not yet practiced |
| Speaking | 5.5 | Not yet practiced |

### Focus Areas
- **Writing Task 1**: 150+ words, 4 paragraphs, linking words
- **Writing Task 2**: Keep practicing, give clear opinion
- **Speaking**: Extend answers to 2+ minutes, reduce filler words
- **Reading/Listening**: Maintain with weekly practice

---

## Key Issues to Address

### Writing Task 1 (Priority)
- **Word count**: User writes ~80-95 words, needs 150+
- **Paragraphs**: No paragraph breaks in essays
- **Linking words**: Missing (Firstly, However, In contrast, Overall)

### Speaking
- **Duration**: Need to extend to 2+ minutes
- **Filler words**: Reduce (um, uh, like)

---

## Band Score Reference

### Writing Task 1 Criteria
| Band | Word Count | Paragraphs | Linking Words | Grammar |
|------|-----------|------------|---------------|---------|
| 5.0 | <100 | None | None | Many errors |
| 5.5 | 100-130 | 1-2 | Few | Some errors |
| 6.0 | 130-150 | 3 | Some | Minor errors |
| 6.5+ | 150+ | 4+ | Good | Few errors |

### Writing Task 2 Criteria
| Band | Word Count | Opinion | Examples | Structure |
|------|-----------|---------|----------|-----------|
| 5.0 | <200 | Unclear | None | Poor |
| 5.5 | 200-230 | Clear | 1 | Basic |
| 6.0 | 230-250 | Clear | 1-2 | Good |
| 6.5+ | 250+ | Clear | 2-3 | Excellent |

---

## Commands Quick Reference

### What Assistant Should Do

1. **Assess practice file**:
   ```bash
   # Read from quiz/{skill}/prompt#.md
   read quiz/writing_task1/prompt3.md
   ```

2. **Update progress.md**:
   - Add to Practice Log table
   - Update Current Estimated Scores

3. **Update dashboard.html**:
   - Add to practiceLog object in script
   - Use skill categories: 'writing_task1', 'writing_task2', 'speaking', 'listening', 'reading'

4. **Add examples to practice file**:
   - Band 6 example (clear, simple)
   - Band 9 example (advanced vocabulary, complex sentences)

5. **Provide next steps**:
   - Focus on biggest issue first
   - Give actionable advice

---

## Study Schedule Reference

### Weekly Practice
| Day | Skill | Target |
|-----|-------|--------|
| Mon | Writing Task 1 | 20 min |
| Tue | Speaking Part 2 | 2 min |
| Wed | Writing Task 2 | 35 min |
| Thu | Listening | 15 min |
| Fri | Writing | Review |
| Sat | Speaking | Part 1 |
| Sun | Review | Progress |

---

*Last Updated: 2026-04-26*
*Assistant should read this file to understand the workflow*