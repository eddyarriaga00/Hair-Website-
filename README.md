# Hair-Website-
 // Prevent double-tap zoom on buttons (mobile fix)
        document.addEventListener('DOMContentLoaded', function() {
            const buttons = document.querySelectorAll('button, .cta-button, .interactive-btn');
            buttons.forEach(button => {
                button.addEventListener('touchend', function(e) {
                    // Prevent zoom on double tap
                    e.preventDefault();
                });
            });
        });