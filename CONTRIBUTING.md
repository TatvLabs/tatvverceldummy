# UI contribution checklist

## Action controls

All new and existing action controls must follow the [mandatory Homebase action-control standard](https://github.com/TatvLabs/homebase/blob/main/docs/standards/action-control-guidance.md). Ordinary navigation links remain links. Homebase issue [#56](https://github.com/TatvLabs/homebase/issues/56) must land before this main-branch standard link resolves.

This documentation adopts the standard. Issue [#7](https://github.com/TatvLabs/tatvverceldummy/issues/7) tracks standard adoption and review of current CTA semantics. The inspected page has no implemented button actions and no semantic button or role="button" controls. Its two CTA anchors use href="#"; this file does not specify their intended destination or whether they are actions. Leave that semantics unresolved until evidenced. Review future implemented actions against the standard; no runtime retrofit is identified where no action is implemented.


## PR review checklist

- [ ] For UI changes, reviewed all new and changed action controls against the [Homebase action-control standard](https://github.com/TatvLabs/homebase/blob/main/docs/standards/action-control-guidance.md).
- [ ] Reviewed the current CTA semantics factually; do not infer a destination or action from href="#" alone.
- [ ] For future implemented action controls, verified next-action tooltip updates across states, action/disclosure names track the action, aria-pressed toggles keep stable names and expose pressed state, and disabled/busy activation is blocked. Record only checks actually performed.
