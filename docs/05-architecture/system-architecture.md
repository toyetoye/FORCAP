# FORCAP System Architecture

## Target Architecture

FORCAP should become one platform with one shell, one access-control model, one vessel registry, one audit trail, and module-based functionality.

## Repository Structure

- `apps/web` - frontend shell
- `apps/api` - backend API
- `modules/core` - users, roles, vessels, access, audit
- `modules/pms` - Engineering / PMS
- `modules/spares` - stores and spare gear
- `modules/finance` - requisitions and budget workflows
- `modules/operations` - EOM, fuel, voyages, work plans
- `modules/compliance` - SIRE, HSSE, refit, claims
- `modules/knowledge` - documents and Oracle
- `packages` - shared libraries
