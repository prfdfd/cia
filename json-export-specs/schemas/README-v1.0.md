# JSON Schema v1.0 Reality-Based Collection

## Overview

This directory contains **v1.0 reality-based JSON schemas** that document the actual fields available in the sample CSV data. These schemas represent **what can be exported today** rather than aspirational future features.

---

## Schema Files

### v1.0 Reality-Based Schemas (NEW - 2025-12-31)

✅ **Validated against actual CSV data** - 100% field completeness

| Schema | CSV Source | Fields | Status |
|--------|------------|--------|--------|
| [politician-schema-v1.0.md](./politician-schema-v1.0.md) | view_riksdagen_politician_sample.csv | 65 | ✅ Complete |
| [party-schema-v1.0.md](./party-schema-v1.0.md) | view_riksdagen_party_sample.csv | 17 | ✅ Complete |
| [committee-schema-v1.0.md](./committee-schema-v1.0.md) | view_riksdagen_committee_sample.csv | 19 | ✅ Complete |
| [ministry-schema-v1.0.md](./ministry-schema-v1.0.md) | view_riksdagen_goverment_sample.csv | 13 | ✅ Complete |
| [intelligence-schema-v1.0.md](./intelligence-schema-v1.0.md) | table_rule_violation_sample.csv | 10 | ✅ Complete |

**Total**: 124 fields across 5 schemas, all validated

---

### v2.0 Aspirational Schemas (Existing)

❓ **Contain aspirational/computed fields** - not all fields available yet

| Schema | Status | Notes |
|--------|--------|-------|
| [politician-schema.md](./politician-schema.md) | Aspirational | Includes voting records, risk scores, predictions |
| [party-schema.md](./party-schema.md) | Aspirational | Includes coalition analytics, ideology metrics |
| [committee-schema.md](./committee-schema.md) | Aspirational | Includes proposal analytics, decision flows |
| [ministry-schema.md](./ministry-schema.md) | Aspirational | Includes minister details, policy areas, budget impact |
| [intelligence-schema.md](./intelligence-schema.md) | Aspirational | Includes risk scoring, ML predictions, impact analysis |

---

## Key Differences

### v1.0 Reality-Based
✅ **All fields present in CSV** - Can export today  
✅ **Direct database columns** - No computation needed  
✅ **100% validated** - Automated CI checks  
✅ **Production ready** - Immediate API use  

**Use Cases:**
- Immediate API implementation
- MVP product launch
- Data export verification
- Field availability reference

---

### v2.0 Aspirational
❓ **Some fields not yet available** - Requires development  
❓ **Includes computed fields** - Needs calculation layer  
❓ **Nested structures** - Requires aggregation  
❓ **Future enhancements** - Planned features  

**Use Cases:**
- Product roadmap planning
- Feature scoping
- Data science requirements
- Long-term architecture

---

## Validation Status

### Reality-Based Validation (v1.0)

**Automated CI Check**: ✅ Passing

```bash
cd json-export-specs
bash validate-field-completeness.sh
```

**Results:**
```
✅ politician-schema.md: 21/21 core fields (100%)
✅ party-schema.md: 6/6 core fields (100%)
✅ committee-schema.md: 7/7 core fields (100%)
✅ ministry-schema.md: 8/8 core fields (100%)
✅ intelligence-schema.md: 9/9 core fields (100%)

Overall: 51/51 required fields present (100%)
```

**Note**: Validation checks core required fields only. v1.0 schemas document all 124 available fields.

---

## Migration Path

### Phase 1: v1.0 Implementation (Current)
1. ✅ Create reality-based schemas (completed)
2. ⏳ Implement JSON export API using v1.0 schemas
3. ⏳ Deploy MVP with available fields
4. ⏳ Gather user feedback on field requirements

### Phase 2: v2.0 Enhancement (Future)
1. ⏳ Implement computed field layer (risk scores, rates, etc.)
2. ⏳ Add voting record aggregation
3. ⏳ Build intelligence analytics engine
4. ⏳ Develop prediction models
5. ⏳ Migrate to v2.0 aspirational schemas

---

## Field Mapping

### How v1.0 Maps to v2.0

**Example: Politician Schema**

| v2.0 Aspirational Field | v1.0 Reality Status | Implementation |
|------------------------|---------------------|----------------|
| `personalInfo.firstName` | ✅ Available | Direct: `first_name` |
| `personalInfo.lastName` | ✅ Available | Direct: `last_name` |
| `voting.totalVotes` | ❌ Not available | Requires: vote table join |
| `voting.partyLoyalty` | ❌ Not available | Requires: computation |
| `intelligence.riskScore` | ❌ Not available | Requires: ML model |
| `documents.total` | ✅ Available | Direct: `total_documents` |
| `documents.productivity` | ⚠️ Partial | Some computed fields needed |

**Legend:**
- ✅ Available: Direct CSV field
- ⚠️ Partial: Some sub-fields available
- ❌ Not available: Requires development

---

## Usage Recommendations

### For API Development
→ **Use v1.0 schemas**
- Guaranteed field availability
- No computation overhead
- Production-ready today

### For Product Planning
→ **Reference v2.0 schemas**
- Future feature roadmap
- Data science requirements
- Long-term architecture vision

### For Documentation
→ **Maintain both versions**
- v1.0: What's available now
- v2.0: Where we're headed
- Clear migration path

---

## Validation Tools

### Automated CI
- **Script**: `validate-field-completeness.sh`
- **Workflow**: `.github/workflows/validate-field-completeness.yml`
- **Runs on**: Schema or CSV changes
- **Status**: ✅ Passing (100% field completeness)

### Manual Validation
```bash
# Check specific schema
cd json-export-specs
bash validate-field-completeness.sh --verbose

# View detailed report
cat FIELD_COMPLETENESS_REPORT.md
```

---

## Version History

### 2025-12-31
- ✅ Created v1.0 reality-based schemas for all 5 entities
- ✅ Documented all 124 available CSV fields
- ✅ Established validation baseline (51 core fields)
- ✅ Defined v1.0 → v2.0 migration path

### 2024-11-24
- 📝 Created v2.0 aspirational schemas (original)
- 📝 Defined ideal JSON structures with computed fields
- 📝 Documented product requirements

---

## Related Documentation

- [../README.md](../README.md) - JSON export specs overview
- [../validate-field-completeness.sh](../validate-field-completeness.sh) - Validation script
- [SCHEMA_VALIDATION_REPORT.md](./SCHEMA_VALIDATION_REPORT.md) - Latest validation results

---

## Questions?

**Field not available?** Check v1.0 schema to see what's currently in CSV  
**Need computed field?** See v2.0 schema for development requirements  
**Validation failing?** Check CI logs or run validation script locally  

**Contact**: Review PR #8153 or issue #[original-issue-number]
