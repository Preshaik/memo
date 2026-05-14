<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<style>
  body { font-family: 'Segoe UI', sans-serif; margin: 0; padding: 20px; background: #fff; }
  .faq-container { max-width: 960px; margin: 0 auto; }
  h2 { color: #8B0000; font-size: 26px; font-weight: 700; margin-bottom: 24px; }
  .faq-section-label {
    font-size: 12px;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.08em;
    color: #8B0000;
    margin: 28px 0 6px 0;
    padding-bottom: 4px;
    border-bottom: 2px solid #8B0000;
  }
  .faq-item { border-bottom: 1px solid #ddd; }
  .faq-question {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 16px 4px;
    cursor: pointer;
    font-size: 15px;
    font-weight: 600;
    color: #1a1a1a;
    user-select: none;
  }
  .faq-question:hover { color: #8B0000; }
  .faq-icon {
    color: #8B0000;
    font-size: 22px;
    font-weight: 400;
    transition: transform 0.3s;
    flex-shrink: 0;
    margin-left: 16px;
  }
  .faq-icon.open { transform: rotate(45deg); }
  .faq-answer {
    display: none;
    padding: 0 8px 18px 4px;
    color: #333;
    font-size: 14.5px;
    line-height: 1.7;
  }
  .faq-answer.open { display: block; }
  .faq-answer ul { margin: 8px 0 0 0; padding-left: 20px; }
  .faq-answer ul li { margin-bottom: 6px; }
</style>
</head>
<body>
<div class="faq-container">
  <h2>Frequently Asked Questions</h2>

  <div class="faq-section-label">Sage Intacct Phase 1</div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">1. What is Sage Intacct Phase 1?<span class="faq-icon">+</span></div>
    <div class="faq-answer">Sage Intacct Phase 1 introduced the new way of handling key finance workflows—especially purchasing and approvals—starting April 1, 2026.</div>
  </div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">2. Who is impacted by Phase 1?<span class="faq-icon">+</span></div>
    <div class="faq-answer">Staff with delegated financial authority and anyone involved in reviewing/approving purchases, invoices, or payments (e.g., Directors, Senior Managers, and other approval authorities). Finance and Accounts Payable (AP) are also directly impacted.</div>
  </div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">3. What is changing about coding in Sage Intacct?<span class="faq-icon">+</span></div>
    <div class="faq-answer">Coding moves into the system. Instead of being written manually on forms and entered by Finance afterward, coding is selected in Sage Intacct as part of the workflow. Approvers can see the coding clearly and can adjust it if needed.</div>
  </div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">4. Does the Procurement Policy still apply?<span class="faq-icon">+</span></div>
    <div class="faq-answer">Yes. The policy remains the same—what changes is how the process is captured and approved in the system.</div>
  </div>

  <div class="faq-section-label">Purchasing</div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">5. What happens for purchases within delegated authority?<span class="faq-icon">+</span></div>
    <div class="faq-answer">Purchases within delegated authority can continue as usual. Once goods/services are delivered, invoices should be sent directly to Accounts Payable for processing.</div>
  </div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">6. What happens for purchases over $10,000?<span class="faq-icon">+</span></div>
    <div class="faq-answer">Purchases over $10,000 must be processed in Sage Intacct using a Purchase Requisition workflow.</div>
  </div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">7. How does the Purchase Requisition (PR) process work?<span class="faq-icon">+</span></div>
    <div class="faq-answer"><ul>
      <li>A Purchase Requisition is submitted in Sage Intacct</li>
      <li>It routes automatically to the appropriate approver</li>
      <li>Supporting documents (quotes, memos, contracts) are uploaded and tracked with the request</li>
      <li>Once approved, it becomes a Purchase Order (PO)</li>
      <li>Future invoices can be matched to the PO for better tracking and control</li>
    </ul></div>
  </div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">8. What documents should be attached to purchasing transactions?<span class="faq-icon">+</span></div>
    <div class="faq-answer">Any required supporting documentation such as quotes, contracts, memos, and other approvals should be attached in the system to avoid delays.</div>
  </div>

  <div class="faq-section-label">Invoice Approvals</div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">9. What is changing about invoice approvals?<span class="faq-icon">+</span></div>
    <div class="faq-answer">Invoice approvals are completed in Sage Intacct instead of through emailed forms or manual routing.</div>
  </div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">10. How do invoice approvals work now?<span class="faq-icon">+</span></div>
    <div class="faq-answer"><ul>
      <li>AP enters the invoice in Sage Intacct (and links it to a PO if applicable)</li>
      <li>The invoice routes to the correct approver</li>
      <li>Approvers review details, coding, and supporting documents in the system</li>
      <li>Approvals are completed digitally</li>
      <li>Documents remain stored with the transaction for audit and reference</li>
    </ul></div>
  </div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">11. Where should vendors send invoices?<span class="faq-icon">+</span></div>
    <div class="faq-answer">Vendors should send invoices directly to Accounts Payable.</div>
  </div>

  <div class="faq-section-label">Payments &amp; Approvals</div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">12. What is changing about EFT approvals?<span class="faq-icon">+</span></div>
    <div class="faq-answer">EFT approvals occur in Sage Intacct. The workflow is system-based, and approvers can review and approve within Intacct.</div>
  </div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">13. What is changing about cheque approvals?<span class="faq-icon">+</span></div>
    <div class="faq-answer">Cheque approvals move to digital authorization in Sage Intacct rather than in-person signing sessions. Supporting documentation is stored with the transaction.</div>
  </div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">14. Can payments proceed without approvals?<span class="faq-icon">+</span></div>
    <div class="faq-answer">No. Payments cannot proceed unless required approvals and earlier workflow steps have been completed.</div>
  </div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">15. Are employee expense claims changing now?<span class="faq-icon">+</span></div>
    <div class="faq-answer">No. The current expense claim form process remains in place for now.</div>
  </div>

  <div class="faq-section-label">Ramp</div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">16. What is Ramp?<span class="faq-icon">+</span></div>
    <div class="faq-answer">Ramp is the upcoming corporate card and spend/expense management platform being introduced through a pilot program.</div>
  </div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">17. Who is in the Ramp pilot group?<span class="faq-icon">+</span></div>
    <div class="faq-answer">A targeted, select group of staff will participate in a time-limited pilot before any wider rollout. If you've been identified, you'll be contacted directly with onboarding details, training, and what to expect.</div>
  </div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">18. Will my spending authority or approval limits change?<span class="faq-icon">+</span></div>
    <div class="faq-answer">No. Ramp does not change what expenses are allowed or who has spending authority. It changes how spending is managed, reviewed, and controlled (with stronger system-based controls and better visibility). During the pilot, workflows, limits, and prompts may be tuned as part of testing and refinement.</div>
  </div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">19. Do I still need to submit receipts the old way?<span class="faq-icon">+</span></div>
    <div class="faq-answer">If you're in the Ramp pilot, receipts will be submitted electronically in Ramp (with prompts and reminders to reduce missing receipts and manual follow-up). If you're not in the pilot, continue using the current receipt/expense process until Ramp is rolled out more broadly.</div>
  </div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">20. How does Ramp connect to Sage Intacct?<span class="faq-icon">+</span></div>
    <div class="faq-answer">Ramp will be used as the corporate card and spend/expense management platform (receipts, approvals, tracking, visibility). Ramp integrates directly with Sage Intacct.</div>
  </div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">21. When will Ramp be rolled out to everyone?<span class="faq-icon">+</span></div>
    <div class="faq-answer">Ramp is being introduced through a pilot first (kick-off late May, pilot launch June 1, pilot use during June–July). Any broader rollout would be determined after the pilot based on results and recommendations.</div>
  </div>

  <div class="faq-section-label">Support &amp; Security</div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">22. Where can I find training and guides?<span class="faq-icon">+</span></div>
    <div class="faq-answer">Use the Finance Training Site / Finance Systems Hub to access training materials and resources.</div>
  </div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">23. How do I get help quickly?<span class="faq-icon">+</span></div>
    <div class="faq-answer">Use the "How to Get Help" support guide (the flow chart) and/or the Finance Training Site support section to route your question to the right person or team.</div>
  </div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">24. How do I confirm an Intacct approval email is legitimate before clicking?<span class="faq-icon">+</span></div>
    <div class="faq-answer">Use this checklist:
      <ul>
        <li>Check the sender email address (confirm the full address, not just the display name)</li>
        <li>The email is system-generated and typically includes "Do not reply" language</li>
        <li>It includes transaction details (requester, document number, date, vendor, amount)</li>
        <li>Hover over links before clicking to ensure the destination looks like your normal Intacct sign-in/tenant link</li>
        <li>When in doubt, do not click—log into Intacct directly to find approvals in your queue</li>
      </ul>
    </div>
  </div>

  <div class="faq-item">
    <div class="faq-question" onclick="toggle(this)">25. What should I do if I think an email looks suspicious?<span class="faq-icon">+</span></div>
    <div class="faq-answer">Do not click any links. Log into Intacct directly and verify if an approval is waiting. If still unsure, contact Finance/IT using the support guide.</div>
  </div>

</div>
<script>
  function toggle(el) {
    var answer = el.nextElementSibling;
    var icon = el.querySelector('.faq-icon');
    answer.classList.toggle('open');
    icon.classList.toggle('open');
  }
</script>
</body>
</html>
