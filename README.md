# akshay-saini-js
Local Storage vs Session Storage
As a Software Engineer,

Why I need to know this?

Responsibility for client-side data: As a developer, you often deal with client-side data storage to enhance user-experience and optimize application performance
User Experience and preferences: Knowing when and how to use local storage or session storage enables you to implement features like remembering user preferences, themes, and customizations
State Management: proper usage contributes to effective state management, that is essential for building responsive and dynamic web applications
Difference between Local Storage and Session Storage

Local Storage:

Persistent storage with no expiration
Larget Storage Capacity (~5-10MB)
Survives Browser restart
Example: Authentication Token, preferences such as light mode/dark mode choice
Session Storage:

Temporary storage for a session
cleared when the session ends(closing tab or browser)
suitable for short-term data needs
Example: data in any online form to be submitted
TradeOffs among options:

Local Storage:
Pros: Persistent data, larger capacity
Cons: Vulnerable to XSS attacks due to accessibility via JavaScirpt, limited by the same-origin policy.
Session Storage:
Pros: clears automatically after the session, better security compared to local storage
cons: Limited lifespan, not suitable for long-term storage
When to Use in Different Scenarios:

Local Storage:
Use when data needs to persist across sessions (e.g., user preferences, authentication tokens).
Suitable for caching resources for improved performance.
Session Storage: - Use for temporary storage during a user's visit (e.g., form data, temporary state information). - Ideal for maintaining state within a single page.
Impact on Application Performance:

Loading Time: - Both storage options are relatively fast, as they operate on the client side and don't involve server requests. - Local storage might have a slight edge in performance due to its larger capacity, but the difference is usually negligible for smaller datasets.

Security: - Both local storage and session storage are accessible via JavaScript, making them vulnerable to XSS attacks. - Avoid storing sensitive information without proper encryption and consider using HttpOnly cookies for critical data.

Storage Capacity:

Local storage provides more storage space, but be cautious not to exceed browser limits (usually around 5-10 MB).
Session storage is limited to the current session, making it suitable for smaller datasets.
Cross-Origin Considerations: - Both local and session storage are subject to the same-origin policy, limiting access to data from different domains for security reasons.
