# Pull Request

## 📌 Summary
Provide a clear description of what this PR does and why it is needed.  
Mention any architectural decisions, refactors, or design considerations if relevant.

---

## 🔗 Related Issue
Link to the related issue or ticket (if applicable).

---

## 🧪 Testing Steps
Describe how you validated this change. Include manual + automated test details.

### **Laravel Validation**
- Commands executed (e.g., `php artisan test`)
- Any seeding or database pre-conditions
- API / controller / job-level behavior verified

### **Filament UI Validation**
- Screens/pages/forms tested  
- Widgets/components verified  
- Actions, tables, filters, exports tested  
- Multi-tenant behavior validated (if applicable)

### **Other Tests**
- Queue/Job execution validated  
- File uploads/import flows tested  
- Background pipelines or schedulers tested  

---

## 🧯 Regression Surface
List any areas that could be affected by this change and what you checked to ensure stability.

---

## 🔒 Security Considerations
- No sensitive data added  
- No internal URLs/keys included  
- No PHI or production identifiers  
- All Laravel policies, gates, and RLS boundaries respected  
- Input validation & sanitization reviewed  

---

## 🧹 Checklist

### **Code Quality**
- [ ] Code follows Laravel & Filament conventions  
- [ ] Code is readable, documented, and commented where needed  
- [ ] No dead code or unused imports  
- [ ] No debugging statements (`dd`, `dump`, `ray`, `logger` leftovers)

### **Static Analysis & CI**
- [ ] PHPStan passes (`vendor/bin/phpstan analyse`)  
- [ ] Pint / formatting applied (`./vendor/bin/pint`)  
- [ ] Tests pass locally  

### **Laravel Application**
- [ ] Migrations are idempotent and reversible  
- [ ] Models/casts/factories updated if required  
- [ ] Queued jobs retry behavior considered  
- [ ] Config/env files NOT changed unless documented

### **Filament Specific**
- [ ] Filament Resources/Pages/RelationManagers tested  
- [ ] Permissions/visibility rules confirmed  
- [ ] Custom widgets or tables validated  
- [ ] Multi-tenant scoping confirmed (if applicable)  
- [ ] Exporters/actions tested for large datasets  

### **Documentation & Release Notes**
- [ ] README or internal docs updated (if needed)  
- [ ] Changelog or release notes entry prepared (if applicable)  

### **Final Review**
- [ ] No breaking changes introduced  
- [ ] PR title follows naming conventions  
- [ ] Screenshots included for UI changes  
- [ ] All acceptance criteria met  

---

## 📸 Screenshots (If UI-related)
Attach before/after screenshots or GIFs to help reviewers understand the change.
