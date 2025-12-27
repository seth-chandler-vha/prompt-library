# Perplexity AI - Persistent Instructions Implementation Guide

**Created:** December 2025  
**Purpose:** Document methods to ensure perplexity-instructions.md directives are applied consistently without manual referencing  
**Canonical Source:** [perplexity-instructions.md](../perplexity-instructions.md)

---

## Executive Summary

This guide documents the optimal methods for implementing persistent custom instructions in Perplexity AI to ensure the comprehensive directives in `perplexity-instructions.md` are consistently applied across all interactions without requiring manual reference in each prompt.

---

## Available Methods for Persistent Instructions

### Method 1: AI Profile Custom Instructions (RECOMMENDED)

**Location:** Settings > Profile  
**Scope:** Global - applies to all searches and interactions  
**Persistence:** Permanent until manually changed  
**Availability:** All Perplexity users (Free and Pro)

#### Implementation Steps:

1. Click your profile icon (top right corner)
2. Select "Settings"
3. Navigate to "Profile" tab
4. Locate "AI Profile" or "Custom Instructions" section
5. Paste the contents of `perplexity-instructions.md` into the custom instructions field
6. Save changes

#### Advantages:
- ✅ Applies universally to all LLMs offered by Perplexity
- ✅ Persists across all conversations and sessions
- ✅ No need to create/manage multiple Spaces
- ✅ Works as system-level prompt for all interactions
- ✅ Simple one-time setup

#### Disadvantages:
- ⚠️ Character limit may apply (typically 2000-4000 characters)
- ⚠️ May need to condense or prioritize key directives
- ⚠️ Cannot be context-specific per topic

#### Best Practices:
- Include the most critical 15 directives from perplexity-instructions.md
- Prioritize: Search-first approach, citation requirements, source quality, reasoning transparency
- Add user context (Deputy Chief of Staff, VA Healthcare, Montana location, SQL expertise)
- Include tone/style preferences (direct, professional, no flattery)
- Reference the FLOORS evaluation criteria

---

### Method 2: Perplexity Spaces with Custom Prompts

**Location:** Library > Spaces  
**Scope:** Space-specific - applies within designated workspace  
**Persistence:** Permanent within each Space  
**Availability:** Perplexity Pro users

#### Implementation Steps:

1. Navigate to Library > Spaces (or create via "Spaces" menu)
2. Click "Create Space" or edit existing Space
3. Configure Space settings:
   - Name: "Professional Research" or "VA Healthcare Analysis"
   - Emoji/Icon: Select relevant identifier
   - AI Model: Choose preferred model (GPT-4, Claude, etc.)
4. Add "Space Instructions" (custom prompt field)
5. Paste relevant sections from `perplexity-instructions.md`
6. Configure domain restrictions if needed
7. Save Space

#### Advantages:
- ✅ Context-specific instructions per Space
- ✅ Can create multiple Spaces for different use cases
- ✅ Supports file uploads and internal knowledge integration
- ✅ Collaboration features (share with team)
- ✅ Domain/source filtering capabilities
- ✅ No practical character limit

#### Disadvantages:
- ⚠️ Requires Pro subscription
- ⚠️ Must remember to work within correct Space
- ⚠️ Instructions don't apply to searches outside the Space
- ⚠️ Requires creating/managing multiple Spaces

#### Recommended Space Structure:

**Space 1: Healthcare Administration**
- Instructions: Healthcare-specific directives, VA context, Joint Commission standards
- Files: VA policies, clinical protocols
- Domain focus: VA.gov, CMS.gov, medical journals

**Space 2: Data Analysis & SQL**
- Instructions: Technical analysis directives, SQL syntax preferences
- Files: Database schemas, data dictionaries
- Focus: Technical documentation, Stack Overflow

**Space 3: Agricultural/Land Management**
- Instructions: Montana-specific context, agricultural focus
- Domain focus: MSU Extension, USDA resources

**Space 4: General Professional Research** (Default)
- Instructions: Core directives from perplexity-instructions.md
- All-purpose research and analysis

---

### Method 3: Perplexity Memory Feature

**Location:** Settings > Personalize > Memory  
**Scope:** Cross-conversation memory (Pro feature)  
**Persistence:** Long-term, stateful memory  
**Availability:** Perplexity Pro users

#### Implementation Steps:

1. Navigate to Settings > Personalize > Memory
2. Enable "Memory" feature
3. Add key facts Perplexity should remember:
   - Professional role and responsibilities
   - Technical expertise and preferences
   - Location and context
   - Behavioral preferences (tone, citation style)

#### Advantages:
- ✅ Persistent across all conversations
- ✅ Automatically applied without Space management
- ✅ Remembers context and preferences

#### Disadvantages:
- ⚠️ Limited to factual information about user
- ⚠️ Cannot store full behavioral instructions
- ⚠️ Items cannot be edited, only added/deleted
- ⚠️ Not suitable for comprehensive instruction sets

#### Best Use Cases:
- User context and background
- Role-specific information
- Location and environmental factors
- Technical skill levels
- Preferred frameworks and standards

---

### Method 4: Templates (Built-in Predefined)

**Location:** Spaces > Templates  
**Scope:** Predefined customizations  
**Persistence:** Template-based  
**Availability:** All users

#### Characteristics:
- Pre-configured instruction sets for common use cases
- Can be used as starting point for custom Spaces
- Limited customization in free tier

#### Use Case:
- Quick setup for standard workflows
- Proof of concept before building custom Space
- Reference for instruction formatting

---

## RECOMMENDED IMPLEMENTATION STRATEGY

### Tier 1: Foundation (Required)

**Setup AI Profile Custom Instructions**

1. Extract the 15 most critical directives from perplexity-instructions.md:
   - Always conduct real-time web searches
   - Cite every factual claim with inline citations
   - Prioritize Tier 1 authoritative sources
   - Show reasoning for complex queries
   - Clarify ambiguities before proceeding
   - Direct, professional tone (no flattery)
   - Apply FLOORS criteria (Truth, Clarity, Stability, Fairness, Humility, Integrity)
   - Reference VA context when relevant
   - Include self-assessment for complex topics
   - Never fabricate data or citations

2. Add user context:
   ```
   Deputy Chief of Staff, Montana VA Health Care System
   Expertise: Healthcare administration, SQL, data analysis, PM&R physician
   Location: Helena, MT
   Preferences: Direct communication, evidence-based approach, actionable recommendations
   ```

3. Character count: Aim for 2000-3000 characters to fit typical limits

### Tier 2: Specialization (Recommended for Pro Users)

**Create 3-4 Purpose-Built Spaces**

1. **Healthcare/Clinical Space** - Full healthcare directives
2. **Data/Analytics Space** - Technical and SQL-focused directives  
3. **General Research Space** - Complete perplexity-instructions.md
4. **Quick Reference Space** - Condensed version for rapid queries

### Tier 3: Optimization (Advanced)

**Enable and Configure Memory Feature**
- Professional background and credentials
- Current projects and initiatives
- Preferred tools and systems (VISTA, CDW, Power BI, Toad)
- Key compliance frameworks (Joint Commission, HEDIS, CMS)

---

## Implementation Checklist

### Phase 1: Initial Setup (15 minutes)
- [ ] Review perplexity-instructions.md in full
- [ ] Extract top 15 priority directives
- [ ] Configure AI Profile custom instructions
- [ ] Test with sample query to verify application
- [ ] Enable Memory feature (Pro users)

### Phase 2: Space Creation (30 minutes, Pro only)
- [ ] Create Healthcare Administration Space
- [ ] Create Data Analysis Space  
- [ ] Create General Research Space
- [ ] Upload relevant files to each Space
- [ ] Configure domain filters where appropriate
- [ ] Test each Space with domain-specific queries

### Phase 3: Refinement (Ongoing)
- [ ] Monitor response quality and directive adherence
- [ ] Adjust AI Profile instructions based on gaps
- [ ] Add Memory items as needed
- [ ] Update Space instructions with lessons learned
- [ ] Document edge cases and refinements

---

## Testing and Validation

### Test Query 1: Healthcare Research
**Query:** "What are the latest Joint Commission standards for stroke center certification?"

**Expected Behavior:**
- Conducts real-time web search
- Cites authoritative sources (Joint Commission, CMS)
- Provides VA-specific context
- Includes actionable recommendations
- Uses professional, direct tone

### Test Query 2: Technical/SQL
**Query:** "Write a SQL query to identify providers with incomplete privileging documentation in the last 90 days."

**Expected Behavior:**
- Shows reasoning and assumptions
- Provides properly formatted SQL code
- Includes error handling considerations
- Notes data validation requirements
- Cites relevant documentation

### Test Query 3: Ambiguous Request
**Query:** "What's the best approach for this problem?"

**Expected Behavior:**
- Asks clarifying questions before proceeding
- Does not make assumptions
- Identifies multiple valid interpretations
- Requests context (VA-specific, clinical, administrative, etc.)

---

## Limitations and Workarounds

### Character Limits in AI Profile
**Problem:** AI Profile may have 2000-4000 character limit

**Workarounds:**
1. Prioritize most critical directives (search-first, citations, sources, tone)
2. Use abbreviated format with bullet points
3. Reference full document: "Follow directives in perplexity-instructions.md in GitHub repo"
4. Supplement with Spaces for detailed use cases

### Instructions Not Applied Consistently
**Problem:** AI occasionally ignores custom instructions

**Workarounds:**
1. Include reminder in prompt: "Apply my custom instructions"
2. Use Spaces instead of global profile for critical workflows
3. Verify instructions are saved properly
4. Report inconsistencies to Perplexity support

### Cannot Edit Memory Items
**Problem:** Memory items can only be added or deleted, not edited

**Workarounds:**
1. Delete incorrect item and add corrected version
2. Be precise when initially adding Memory items
3. Use AI Profile for behavioral instructions instead

---

## Maintenance and Updates

### Monthly Review
- Check if perplexity-instructions.md has been updated
- Verify custom instructions still reflect current directives
- Update Spaces with any new frameworks or standards
- Add new Memory items for evolving context

### When to Update Instructions
- New compliance requirements (Joint Commission, CMS)
- Changes to VA policies or systems
- Addition of new technical skills or tools
- Changes to professional responsibilities
- Feedback indicates directive gaps

### Version Control
- Document date of last sync with perplexity-instructions.md
- Track changes made to AI Profile instructions
- Maintain changelog of Space modifications
- Note any deviations from canonical source

---

## Troubleshooting

### Issue: Responses don't follow instructions
**Diagnosis:**
1. Verify instructions are saved in Settings > Profile
2. Check character count hasn't exceeded limit
3. Confirm you're working in correct Space (if using Spaces)
4. Test with explicit prompt referencing instructions

**Resolution:**
- Re-save AI Profile instructions
- Condense to fit character limit
- Switch to appropriate Space
- Contact Perplexity support if persistent

### Issue: Instructions conflict with query
**Diagnosis:**
- Overly prescriptive instructions may limit flexibility
- Context-specific needs may override general directives

**Resolution:**
- Use prompt override: "For this query, ignore tone preferences..."
- Create specialized Space for unique use cases
- Add conditional language to instructions ("unless specified otherwise")

---

## References and Resources

### Internal Documentation
- [perplexity-instructions.md](../perplexity-instructions.md) - Canonical instruction source
- [masterpromptinstructions.md](../masterpromptinstructions.md) - Universal prompt guidelines

### External Resources
- [Perplexity Help Center - Profile Settings](https://www.perplexity.ai/help-center/en/articles/10352993-profile-settings)
- [Perplexity Blog - Introducing Spaces](https://www.perplexity.ai/hub/blog/introducing-internal-knowledge-search-and-spaces)
- [Perplexity Prompt Guide](https://docs.perplexity.ai/guides/prompt-guide)

---

## Conclusion

The optimal approach combines multiple methods:

1. **AI Profile Custom Instructions** (global baseline)
2. **Perplexity Spaces** (context-specific deep work)
3. **Memory Feature** (persistent user context)

This layered strategy ensures comprehensive directive application while maintaining flexibility for specialized workflows.

**Next Steps:**
1. Implement Tier 1 (AI Profile) immediately
2. Create Spaces for top 3 use cases (Pro users)
3. Enable and populate Memory feature
4. Test and refine over 2-week period
5. Document lessons learned and update this guide

---

**Document Status:** Initial version  
**Last Updated:** December 27, 2025  
**Next Review:** January 27, 2026
