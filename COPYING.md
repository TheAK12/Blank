# BLANK Browser License Guide

## Plain English Explanation of MPL 2.0

### What is BLANK Browser?

**BLANK Browser** is a minimalist, privacy-first web browser designed for human-centered interaction, keyboard-driven efficiency, and radical simplicity. It's licensed under the **Mozilla Public License 2.0 (MPL 2.0)**, the same license used by Firefox.

---

## What Can You Do?

### ✅ You CAN:

**Use BLANK Browser for any purpose**
- Personal use
- Commercial projects
- Educational purposes
- Research and development
- Contribution to the project

**Modify the code**
- Customize features to your needs
- Fix bugs you discover
- Optimize performance
- Adapt to your use case

**Distribute BLANK Browser**
- Share it with others
- Include it in your products
- Offer it as a service
- Sell software that uses BLANK

**Combine with proprietary software**
- Create a commercial product using BLANK
- Add proprietary features on top
- Mix BLANK code with closed-source code
- Build business models around BLANK

---

## What Must You Do?

### 📋 You MUST:

**Include the license notice**
- Copy the LICENSE file to any distribution
- Include copyright attribution
- Don't remove or obscure license notices

**Keep modified BLANK files open-source**
- If you modify BLANK's source code and distribute it, those modifications must remain under MPL 2.0
- Others must have the same rights you received
- You can't close-source BLANK's core

**Provide source code availability**
- If you distribute compiled/executable versions, make source code available
- Either include it directly or provide instructions on how to get it
- No charge beyond reasonable distribution cost

**Document your changes**
- Clearly identify what you modified
- Make it obvious which files are your modifications
- Help others understand the changes

---

## What CAN'T You Do?

### ❌ You CANNOT:

**Remove or hide the license**
- You must preserve license notices
- Can't claim you created BLANK if you didn't
- Must acknowledge original contributors

**Restrict others' rights**
- You can't take away rights the license grants
- Can't use patents to block derivatives
- Can't prevent others from modifying your modifications

**Use BLANK's trademarks misleadingly**
- Can't use "BLANK Browser" for your version without permission
- Can't falsely represent your fork as official
- Must distinguish derivatives clearly

**Hold contributors liable**
- BLANK is provided "as-is"
- Contributors aren't liable for damages
- You assume all risks using BLANK

---

## Understanding MPL 2.0: File-Level Copyleft

### The Key Concept

MPL 2.0 is a "weak copyleft" license. This means:

**Modified BLANK files → must stay open**
```
Your Project:
├── browser-engine.ts (from BLANK, modified) → MUST be open-source
├── keyboard-handler.ts (from BLANK, unmodified) → MUST be open-source
├── your-proprietary-feature.ts (you created) → can stay proprietary ✓
└── your-payment-system.js (you created) → can stay proprietary ✓
```

**Unlike GPL**, MPL 2.0 doesn't force your entire project to be open.

### Example: Building a Service on BLANK

**Scenario**: You want to create a commercial browser service using BLANK.

```
Your Commercial Browser Service:
│
├── BLANK Core Browser (MPL 2.0)
│   ├── engine.ts (modified by you) → Open-source, MPL 2.0
│   ├── keyboard-handler.ts (modified by you) → Open-source, MPL 2.0
│   └── privacy-engine.ts (unmodified) → Open-source, MPL 2.0
│
└── Your Proprietary Layer
    ├── Cloud sync service → Proprietary, your license
    ├── Premium themes → Proprietary, your license
    ├── Ad-removal service → Proprietary, your license
    └── Custom integrations → Proprietary, your license

Result:
✅ Users get free, open-source browser core
✅ You make money from proprietary services
✅ Community can audit security and privacy
✅ Improvements to core flow back to BLANK
```

---

## Use Cases

### Case 1: Contributing Improvements

**You**: Fix a bug in BLANK's keyboard handler
**You must**: 
- Share your fix with the community
- It goes under MPL 2.0
- Others can use your improvement

**You get**:
- Credit for the contribution
- Right to use BLANK in your projects
- Community recognition

### Case 2: Creating a Browser Fork

**You**: Want to create a specialized browser based on BLANK
**You can**:
- Modify BLANK's code
- Add custom features
- Distribute your version

**You must**:
- Keep modified BLANK files open-source
- Include the license
- Attribute original BLANK work

**You can also**:
- Add proprietary plugins
- Build proprietary services on top
- Sell your browser

### Case 3: Using BLANK in Your App

**You**: Want to embed BLANK in your desktop application
**You can**:
- Use BLANK's code in your app
- Add it to your proprietary project
- Monetize your application

**You must**:
- Include BLANK's license
- Make source code available
- Give attribution

**You can also**:
- Close-source your app's other parts
- Charge for your app
- Not release your app's source

### Case 4: Academic Research

**You**: Research browser security
**You can**:
- Study BLANK's code
- Publish papers about it
- Create modifications
- Share findings with community

**You should**:
- Attribute BLANK
- Share back improvements
- Contribute security fixes

---

## Patent Protection

### How Patents Work in MPL 2.0

**Automatic grant**: When you contribute code to BLANK, you automatically grant patent rights to:
- All users of BLANK
- All users of derivatives
- The entire community

**Protection for users**: You can't later sue someone for using BLANK based on patents, because you already granted rights.

**Protection for contributors**: You're protected from patent claims by other contributors to BLANK.

**Why this matters**: Prevents patent wars from destroying open-source projects.

---

## Trademark Usage

### Using the "BLANK Browser" Name

**You can**:
- Use "BLANK" to describe derivatives ("Based on BLANK")
- Acknowledge the source project
- Reference BLANK in documentation

**You must**:
- Not claim your fork is the official BLANK
- Clearly distinguish your version
- Give proper attribution

**Example**:
- ✅ "My Browser" (powered by BLANK Engine)
- ✅ "BLANK Browser - Community Fork"
- ❌ "BLANK Browser" (if you've forked significantly)
- ❌ Claiming your version is the "official" BLANK

---

## Contributing Back to BLANK

### Sharing Your Improvements

**Why contribute?**
- Improves BLANK for everyone
- Reduces maintenance burden for you
- Strengthens the community
- Your name in contributor list

**How to contribute**:
1. Fork BLANK on GitHub
2. Make your changes
3. Create a pull request
4. Submit your contribution
5. Community review and merge

**What happens**:
- Your code stays under MPL 2.0
- You retain original authorship
- BLANK community benefits from improvements
- You get credit and recognition

---

## Frequently Asked Questions

### Q: Is BLANK Browser really free?

**A**: Yes, absolutely free.
- No cost to use
- No restrictions on redistribution
- Community-driven development
- No licensing fees

### Q: Can a company use BLANK for commercial products?

**A**: Yes, completely.
- Companies can build on BLANK
- You can sell products using BLANK
- You just can't restrict others' rights to the source

### Q: What if BLANK gets integrated into another project?

**A**: That's encouraged!
- Other projects can use BLANK
- Mergers and integrations are allowed
- Improvements flow both directions

### Q: Can someone steal BLANK and make it proprietary?

**A**: No, they can't "steal" it because:
- Modified BLANK code must stay open
- Users get source code
- License prevents proprietary versions
- Community can audit and verify

### Q: Why MPL 2.0 instead of MIT or GPL?

**A**: MPL 2.0 balances:
- **Community needs**: Ensures improvements flow back
- **Commercial viability**: Allows proprietary layers
- **Simplicity**: File-level copyleft (not "viral" like GPL)
- **Precedent**: Used by Firefox, Mozilla products

### Q: What if I don't follow the license?

**A**: 
- Your rights terminate automatically
- You lose all BLANK usage rights
- Others can still distribute their versions
- You'd be in legal violation

### Q: Can the license change in the future?

**A**: 
- Only Mozilla Foundation can change MPL 2.0 itself
- BLANK can adopt a new version of MPL
- Existing code stays under current license
- You're not forced to upgrade

### Q: What about security vulnerabilities?

**A**: 
- Report privately to security team
- Don't disclose publicly until patch
- License allows emergency patches
- Community can security audit code

---

## Legal Summary

### Rights Granted to You

| Right | Status |
|-------|--------|
| Use for any purpose | ✅ Granted |
| Modify the code | ✅ Granted |
| Distribute copies | ✅ Granted |
| Commercial use | ✅ Granted |
| Create Larger Works | ✅ Granted |
| Patent rights | ✅ Granted |
| Sublicense | ✅ Granted (with conditions) |

### Obligations You Accept

| Obligation | Status |
|-----------|--------|
| Include license notice | ✅ Required |
| Preserve copyright notices | ✅ Required |
| Keep modified files open | ✅ Required |
| Provide source code | ✅ Required |
| Document changes | ✅ Required |
| Attribute original work | ✅ Required |

### Limitations (What You DON'T Get)

| Limitation | Status |
|-----------|--------|
| Warranty (as-is) | ⚠️ Disclaimed |
| Liability protection | ⚠️ Limited |
| Trademark rights | ✅ Separate agreement needed |
| Patent indemnity | ✅ Not guaranteed (beyond contributor grants) |

---

## Resources

- **Full License Text**: See [LICENSE](./LICENSE) file
- **Mozilla Public License FAQ**: https://www.mozilla.org/en-US/MPL/2.0/FAQ/
- **Open Source Initiative**: https://opensource.org/
- **BLANK Browser Repository**: https://github.com/[username]/blank-browser

---

## Questions?

Have questions about how MPL 2.0 applies to BLANK Browser?

- **GitHub Issues**: Open an issue on the repository
- **Discussions**: Use GitHub Discussions for general questions
- **Legal**: Consult a lawyer for specific legal advice
- **Community**: Ask in our community forum

---

## Philosophy Behind This License

BLANK Browser is more than code—it's a philosophy about design, privacy, and human autonomy.

**MPL 2.0 protects this philosophy by ensuring**:
- ✅ Core principles remain open to inspection
- ✅ Privacy features stay community-auditable
- ✅ Design principles are preserved for all
- ✅ Improvements benefit everyone
- ✅ Commercial viability doesn't compromise values

**We chose MPL 2.0 because**:
- Firefox uses it (proven for large browser projects)
- It balances community good with practical adoption
- It prevents proprietary forks that hide tracking
- It enables commercial businesses to build on BLANK
- It respects contributor autonomy

---

## Contributing and Joining BLANK

### We Welcome

- 🎨 **Designers**: Improve the interface
- 💻 **Developers**: Implement features
- 🔒 **Security experts**: Audit and enhance privacy
- ♿ **Accessibility advocates**: Improve WCAG compliance
- 📚 **Documentation writers**: Improve guides
- 🧪 **Testers**: Find and report bugs
- 🤔 **Researchers**: Study and publish findings

### Getting Started

1. Read the [CONTRIBUTING.md](./CONTRIBUTING.md) guide
2. Check out [good-first-issue](https://github.com/[username]/blank-browser/labels/good-first-issue) tags
3. Join [GitHub Discussions](https://github.com/[username]/blank-browser/discussions)
4. Fork the repository and make your first contribution

---

## Final Note

BLANK Browser is free, open-source software. This license ensures that freedom while enabling commercial innovation. 

**Design by Subtraction. Built by Community. Yours to modify.**

---

*Last updated: November 2, 2025*
*License version: Mozilla Public License 2.0*
