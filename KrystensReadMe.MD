In auditing the site, I used lighthouse on Google Chrome to run the accessibility analysis. The score came out to 83. In looking at the audit, I saw:
    
    - Contrast: Background and foreground colors do not have a sufficient contrast ratio.
    - Navigation: Heading elements are not in a sequentially-descending order.
    - Best practices: Document does not have a main landmark.

Changes I made:
    - Replaced <div class="content"> with <main class="content">
    - Removed <div class="hero">, replaced with <header class="header"> and closed with </header>
    - Removed <div class="footer"> and replaced it with <footer class="footer">
    - Removed <div class="nav"> and replaced with <nav class="nav">
    - Replaced <div class="form-section"> with <section class="form-section">
    - Replaced h3 tags with h2 tags because they need to be sequenced properly
    - Added more contrasting colors to the nav, footer, and body


    After all of these changes, the site score now sits at 100. 