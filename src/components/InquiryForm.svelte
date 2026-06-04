<section id="inquiry-section" class="inquiry-container">
  <h3>Have questions about the Vaelia pilot?</h3>
  <form action="https://formspree.io/f/maqklked" method="POST" class="inquiry-form">
    <input type="text" name="name" placeholder="Your Name" required />
    <input type="email" name="email" placeholder="Your Email" required />
    <textarea name="challenge" placeholder="What technical communication challenge are you facing?" required></textarea>
    <label>
      <input type="checkbox" name="request-audit" />
      Send me the Free Technical Communication Audit PDF
    </label>
    <button type="submit" class="btn-enroll">Send Inquiry</button>
  </form>
</section>

<style>
  .inquiry-container {
    padding: 4rem 2rem;
    max-width: 600px;
    margin: 0 auto;
    text-align: center;
  }
  .inquiry-container h3 {
    font-size: 1.5rem;
    margin-bottom: 1.5rem;
    color: #f8fafc;
    font-family: 'Outfit', sans-serif;
  }
  .inquiry-form {
    display: flex;
    flex-direction: column;
    gap: 1rem;
  }
  input[type="text"], input[type="email"], textarea {
    padding: 0.8rem;
    background-color: #0f172a;
    border: 1px solid #1e293b;
    color: #f8fafc;
    border-radius: 8px;
    outline: none;
    font-family: 'Inter', sans-serif;
    transition: border-color 0.2s, hover-border-color 0.2s;
  }
  input[type="text"]:hover, input[type="email"]:hover, textarea:hover {
    border-color: rgba(0, 142, 137, 0.4);
  }
  input[type="text"]:focus, input[type="email"]:focus, textarea:focus {
    border-color: #008e89;
  }
  textarea {
    resize: none;
    height: 120px;
  }
  label {
    display: flex;
    align-items: center;
    gap: 0.5rem;
    color: #94a3b8;
    font-size: 0.875rem;
    cursor: pointer;
    text-align: left;
    user-select: none;
  }
  .btn-enroll {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    background-color: #008e89;
    color: #f8fafc;
    font-family: 'Outfit', sans-serif;
    font-weight: 600;
    border-radius: 8px;
    padding: 0.75rem 1.5rem;
    transition: all 0.2s ease-in-out;
    box-shadow: 0 4px 14px 0 rgba(0, 142, 137, 0.3);
    border: none;
    cursor: pointer;
    font-size: 1rem;
  }
  .btn-enroll:hover {
    background-color: #00b0aa;
    transform: translateY(-1px);
    box-shadow: 0 6px 20px 0 rgba(0, 142, 137, 0.45);
  }
</style>
