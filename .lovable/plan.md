
# PMER-MIS — UI Prototype Plan

## Overview
Build a frontend-only demo of the ERCS Planning, Monitoring, Evaluation & Reporting system with realistic mock data. Clean, modern SaaS-style design with sidebar navigation. No backend — all data is hardcoded/mock for stakeholder review.

## Layout & Navigation
- **Sidebar** with collapsible icon mode using shadcn Sidebar component
- ERCS branding (red accent color, logo placeholder)
- Top header with user avatar, notifications bell, and sidebar trigger
- Main sections in sidebar: Dashboard, Planning, Monitoring, Budget, Reports, Users, Documents

## Pages & Modules

### 1. Dashboard (Home)
- KPI summary cards: total branches, active projects, budget utilization %, indicator achievement %
- Traffic light summary (green/yellow/red counts)
- Top 5 underperforming indicators table
- Budget burn rate gauge chart
- Recent activity feed

### 2. Planning Module
- **AOP List View**: Table of Annual Operational Plans with status badges (Draft, Submitted, Approved)
- **AOP Detail/Builder**: Tabbed view with Objectives → Activities → Budget → Logframe
- **Gantt Chart**: Visual timeline of activities with milestone markers using a simple CSS/SVG Gantt
- **Logframe Viewer**: Hierarchical tree showing Strategic Priority → Outcome → Output → Activity linkages
- Quarterly plan view with planned vs actual comparison

### 3. Indicator Monitoring Module
- **Indicator Registry**: Searchable/filterable table of indicators with type badges (Output/Outcome/Impact)
- **Data Entry View**: Form-style monthly entry with validation indicators
- **Performance Dashboard**: 
  - Achievement % bar charts by branch
  - Traffic light grid (indicators × branches)
  - Trend sparklines
- **Indicator Detail**: Target vs achievement chart, disaggregation breakdown, variance explanation history

### 4. Budget & Financial Module
- **Budget Overview**: Summary cards (total budget, spent, remaining, burn rate)
- **Budget vs Expenditure Table**: By activity/project with progress bars
- **Donor Allocation View**: Multi-donor split visualization
- **Cost Efficiency Metrics**: Cost per beneficiary, cost per output cards
- **Variance Analysis**: Bar chart comparing planned vs actual by quarter

### 5. User Management
- **User List**: Table with role badges, branch assignment, last login
- **Role Matrix**: Grid showing permissions per role (Super Admin, PMER Admin, Branch Admin, Data Entry, Finance, Read-only)
- **Audit Log**: Timestamped log of user actions (mock entries)

### 6. Reports (Read-only preview)
- List of report templates (Monthly, Quarterly, Semi-annual, Annual, Donor-specific)
- Sample generated report preview with export buttons (PDF/Excel/Word — non-functional, just UI)

## Mock Data
- 6 ERCS branches (Addis Ababa, Amhara, Oromia, SNNPR, Tigray, Somali)
- 3 sample projects with donor tags (IFRC, ICRC, Norwegian Red Cross)
- ~15 indicators with disaggregation data
- Budget data across quarters with realistic variance
- 10 mock users across all roles

## Design System
- Clean white background, subtle gray borders
- ERCS red (#D32F2F) as primary accent
- Traffic light colors: green (#4CAF50), yellow (#FF9800), red (#F44336)
- shadcn components throughout (tables, cards, tabs, badges, charts)
- Recharts for all data visualizations
- Responsive — works on tablet and desktop
