# FORCAP PMS Requirements

## Purpose

The FORCAP Engineering/PMS module shall replace the core PROP Engineering planned maintenance workflows.

This module is the first serious FORCAP replacement target because it is operationally critical and likely to become the first Class-facing part of the product.

## PMS Product Goal

FORCAP PMS shall allow ship and shore users to:

- maintain a vessel-specific equipment/component registry
- define planned maintenance jobs
- issue worksheets
- complete maintenance work
- defer work under controlled conditions
- record running hours
- record ad-hoc maintenance
- require Chief Engineer authorisation
- preserve completed maintenance history
- produce familiar PMS reports
- provide audit and Class evidence

## Baseline PMS Record Requirements

A completed worksheet record shall preserve, at minimum:

- tenant/customer
- vessel
- vessel official number, where applicable
- component code
- component name
- component criticality group
- job code
- job description
- job type
- original due date
- deferred-until date, where applicable
- date completed
- completed by rank
- completed by person
- Chief Engineer authorisation/sign-off
- completion comments
- running hours, where applicable
- attachments, where applicable
- audit trail

## Functional Requirements

### PMS-001 Component Registry

FORCAP shall maintain a vessel-specific component registry.

### PMS-002 Component Hierarchy

FORCAP shall support a hierarchy of vessel, system/group, assembly, component, PM template, issued worksheet, completed worksheet, spares, files, and history.

### PMS-003 Component Criticality

FORCAP shall support Critical, Significant, and Standard component grouping.

### PMS-004 PM Worksheet Templates

FORCAP shall support planned maintenance worksheet templates with job code, description, frequency, assigned rank, job type, measurements, attachments, spares, active status, and revision history.

### PMS-005 Issued Worksheets

FORCAP shall issue worksheets from PM templates based on calendar interval, running hours, condition-based requirement later, or manual issue by authorised user.

### PMS-006 Deferral Workflow

FORCAP shall allow authorised users to defer worksheets with reason, new deferred-until date or running-hour counter, audit event, and report visibility.

### PMS-007 Completion Workflow

FORCAP shall allow assigned or authorised users to complete worksheet records with completion date, person, rank, work comments, measurements, running hours, parts used, and attachments where applicable.

### PMS-008 Chief Engineer Authorisation

FORCAP shall require Chief Engineer or authorised role review before a completed worksheet enters final maintenance history.

### PMS-009 Return Workflow

FORCAP shall allow the Chief Engineer or authorised role to return a completed worksheet for correction with a mandatory reason.

### PMS-010 Completed Worksheet History

FORCAP shall preserve completed worksheet history by vessel, component, job, date range, rank/person, criticality, job type, and due/completed/deferred status.

### PMS-011 Ad-hoc Maintenance

FORCAP shall allow users to enter ad-hoc maintenance reports linked to vessel, component where applicable, responsible rank/person, date completed, description, attachments, and related defect/action in a later phase.

### PMS-012 Running Hours

FORCAP shall record running hours and support running-hour-based maintenance triggers.

### PMS-013 PMS Reports

Initial PMS reports shall include Completed Worksheets by Component, Completed Worksheets by Job, Issued Worksheets, Deferred Worksheets, Overdue Worksheets, Worksheets Awaiting Authorisation, Running Hours Sheet, Component History, Ad-hoc Maintenance History, Critical Component Maintenance History, Significant Component Maintenance History, and Maintenance Forecast.

## Non-functional Requirements

- All critical PMS actions shall be audited.
- Access shall be controlled by user, role, vessel, module, and action.
- PMS history shall be immutable after authorisation except through a controlled correction/revision process.
- Reports shall be exportable.
- The system shall support future Class evidence requirements.
- The system shall support shipboard low-connectivity workflows later through draft/autosave and sync status.
