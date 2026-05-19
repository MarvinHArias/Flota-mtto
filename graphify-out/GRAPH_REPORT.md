# Graph Report - .  (2026-05-19)

## Corpus Check
- 112 files · ~73,262 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 552 nodes · 791 edges · 60 communities (47 shown, 13 thin omitted)
- Extraction: 90% EXTRACTED · 10% INFERRED · 0% AMBIGUOUS · INFERRED: 81 edges (avg confidence: 0.77)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- [[_COMMUNITY_Community 0|Community 0]]
- [[_COMMUNITY_Community 1|Community 1]]
- [[_COMMUNITY_Community 2|Community 2]]
- [[_COMMUNITY_Community 3|Community 3]]
- [[_COMMUNITY_Community 4|Community 4]]
- [[_COMMUNITY_Community 5|Community 5]]
- [[_COMMUNITY_Community 6|Community 6]]
- [[_COMMUNITY_Community 7|Community 7]]
- [[_COMMUNITY_Community 8|Community 8]]
- [[_COMMUNITY_Community 9|Community 9]]
- [[_COMMUNITY_Community 10|Community 10]]
- [[_COMMUNITY_Community 11|Community 11]]
- [[_COMMUNITY_Community 12|Community 12]]
- [[_COMMUNITY_Community 13|Community 13]]
- [[_COMMUNITY_Community 14|Community 14]]
- [[_COMMUNITY_Community 15|Community 15]]
- [[_COMMUNITY_Community 16|Community 16]]
- [[_COMMUNITY_Community 17|Community 17]]
- [[_COMMUNITY_Community 18|Community 18]]
- [[_COMMUNITY_Community 19|Community 19]]
- [[_COMMUNITY_Community 20|Community 20]]
- [[_COMMUNITY_Community 22|Community 22]]
- [[_COMMUNITY_Community 23|Community 23]]
- [[_COMMUNITY_Community 24|Community 24]]
- [[_COMMUNITY_Community 26|Community 26]]
- [[_COMMUNITY_Community 27|Community 27]]
- [[_COMMUNITY_Community 29|Community 29]]
- [[_COMMUNITY_Community 36|Community 36]]
- [[_COMMUNITY_Community 37|Community 37]]
- [[_COMMUNITY_Community 38|Community 38]]
- [[_COMMUNITY_Community 39|Community 39]]
- [[_COMMUNITY_Community 40|Community 40]]
- [[_COMMUNITY_Community 41|Community 41]]
- [[_COMMUNITY_Community 48|Community 48]]
- [[_COMMUNITY_Community 49|Community 49]]

## God Nodes (most connected - your core abstractions)
1. `APIClient` - 44 edges
2. `FlotaApp` - 32 edges
3. `OfflineDB` - 11 edges
4. `OrderSchedule` - 10 edges
5. `User` - 10 edges
6. `SyncManager` - 9 edges
7. `map_order_to_response()` - 8 edges
8. `_role()` - 8 edges
9. `get_password_hash()` - 8 edges
10. `StockMovement` - 8 edges

## Surprising Connections (you probably didn't know these)
- `create_planner()` --calls--> `get_password_hash()`  [INFERRED]
  scripts/create_planner.py → app/core/security.py
- `import_technicians()` --calls--> `get_password_hash()`  [INFERRED]
  scripts/import_technicians.py → app/core/security.py
- `reset_users()` --calls--> `get_password_hash()`  [INFERRED]
  scripts/reset_users.py → app/core/security.py
- `seed_manager()` --calls--> `get_password_hash()`  [INFERRED]
  scripts/seed_manager.py → app/core/security.py
- `seed_stock_movements()` --calls--> `Product`  [INFERRED]
  scripts/seed_stock_movements.py → app/models/inventory.py

## Communities (60 total, 13 thin omitted)

### Community 0 - "Community 0"
Cohesion: 0.00
Nodes (50): Base, Enum, MovementType, Product, PurchaseOrder, PurchaseOrderItem, PurchaseStatus, StockMovement (+42 more)

### Community 1 - "Community 1"
Cohesion: 0.00
Nodes (53): BaseModel, Config, Token, TokenData, UserCreate, UserResponse, ChecklistCreate, ChecklistDetail (+45 more)

### Community 3 - "Community 3"
Cohesion: 0.00
Nodes (14): FlotaApp, MENU_CONFIG, renderMenuForRole(), AI_CONFIG, animateCounter(), handleChatKeypress(), initAIDashboard(), renderAIView() (+6 more)

### Community 4 - "Community 4"
Cohesion: 0.00
Nodes (24): _extract_token(), get_current_user(), get_db(), Shared API dependencies., Database session dependency, Get current authenticated user from JWT token (header or cookie)., create_access_token(), decode_access_token() (+16 more)

### Community 5 - "Community 5"
Cohesion: 0.00
Nodes (17): Unit, Config, UnitBase, UnitCreate, UnitFlota360, UnitResponse, UnitTimelineItem, UnitUpdate (+9 more)

### Community 6 - "Community 6"
Cohesion: 0.00
Nodes (15): ensure_self_or_roles(), Checklist, ensure_file_size(), validate_upload(), _can_access_checklist(), create_checklist(), get_checklist(), get_checklist_media() (+7 more)

### Community 7 - "Community 7"
Cohesion: 0.00
Nodes (15): adjustStock(), changePOStatus(), handleInventorySearch(), inventoryFilters, loadWarehouseData(), openNewProductModal(), openNewPurchaseModal(), renderCurrentTab() (+7 more)

### Community 8 - "Community 8"
Cohesion: 0.00
Nodes (8): approveOrderAction(), closeOrderModal(), deleteOrderAction(), handleCreateOrderSubmit(), loadTechniciansForOrder(), loadUnitsForOrder(), rejectOrderAction(), showCreateOrderForm()

### Community 9 - "Community 9"
Cohesion: 0.00
Nodes (11): applyAuditFilters(), auditData, closeAuditModal(), loadAuditHistory(), markAsPriority(), renderAuditView(), renderNoInspectionView(), renderPriorityButton() (+3 more)

### Community 10 - "Community 10"
Cohesion: 0.00
Nodes (12): closeUnitDetailModal(), closeUnitModal(), confirmDeleteUnit(), filter, input, loadFlota360Data(), loadUnitTimeline(), options (+4 more)

### Community 11 - "Community 11"
Cohesion: 0.00
Nodes (10): closeUserModal(), confirmDeleteUser(), escapeHTML(), filterUsers(), loadUsersData(), renderUsersView(), showUserDetailModal(), submitCreateUser() (+2 more)

### Community 13 - "Community 13"
Cohesion: 0.00
Nodes (10): clean_for_json(), get_llantas_excel(), get_servicios_excel(), get_tire_status(), parse_tire_value(), Recursively clean data for JSON serialization, Parse tire measurement value, removing letters and extracting number, Get status based on millimeters: <=4 critical (red), 5-6 warning (yellow), >6 go (+2 more)

### Community 14 - "Community 14"
Cohesion: 0.00
Nodes (9): attachPlannerHandlers(), attachTechnicianHandlers(), _currentTechOrders, loadOrdersData(), loadTechnicianStats(), renderOrdersView(), renderPlannerOrdersView(), renderTechnicianOrdersView() (+1 more)

### Community 16 - "Community 16"
Cohesion: 0.00
Nodes (9): background_color, description, display, icons, name, orientation, short_name, start_url (+1 more)

### Community 17 - "Community 17"
Cohesion: 0.00
Nodes (9): filterByCuenta(), loadTiresData(), renderTireBox(), renderTiresView(), renderTiresVisualMap(), renderTop10Critical(), renderUnitTireCard(), tiresState (+1 more)

### Community 18 - "Community 18"
Cohesion: 0.00
Nodes (8): build_insert_or_upsert_sql(), clear_target_data(), count_rows(), existing_tables(), main(), migrate_table(), migrate_users_and_units(), reset_sequences()

### Community 19 - "Community 19"
Cohesion: 0.00
Nodes (7): loadDashboardKPIs(), loadExternalData(), loadLiveActivity(), loadTodayWorkload(), loadTopExpensiveParts(), loadTopPartsConsumed(), renderDashboardWithKPIs()

### Community 22 - "Community 22"
Cohesion: 0.00
Nodes (5): downgrade(), _has_column(), _has_fk(), _has_table(), upgrade()

### Community 23 - "Community 23"
Cohesion: 0.00
Nodes (4): Run migrations in 'offline' mode.      This configures the context with just a U, Run migrations in 'online' mode.      In this scenario we need to create an Engi, run_migrations_offline(), run_migrations_online()

### Community 26 - "Community 26"
Cohesion: 0.00
Nodes (3): _auth_header(), test_create_and_get_unit(), test_create_duplicate_unit()

### Community 27 - "Community 27"
Cohesion: 0.00
Nodes (3): BaseSettings, Config, Settings

### Community 29 - "Community 29"
Cohesion: 0.00
Nodes (3): downgrade(), _has_column(), upgrade()

## Knowledge Gaps
- **31 isolated node(s):** `Config`, `Config`, `Config`, `Config`, `Config` (+26 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **13 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.