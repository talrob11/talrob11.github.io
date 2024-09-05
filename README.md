Variables: 
navBar: Selects the navigation bar element with the class .navbar__menu.
navList: Selects the unordered list within the navigation bar with the ID #navbar__list.
sections: Selects all section elements on the page.
footer: Selects the footer element.
header: Selects the header element with the class .page__header.

Navigation:
buildNav: A function that creates navigation buttons for each section.
Loops through each section and creates a list item (li).
Inserts an anchor (a) element inside the list item, setting the href attribute to the section's ID and the text to the section's data-nav attribute.
Appends each list item to the navigation list (navList).
Calls scrollBehavior to add smooth scrolling to each navigation button.
Finally, appends the populated navList to the navBar.

Scroll Behavior:
scrollBehavior: Adds smooth scrolling behavior to each navigation button.
Adds a click event listener to each navigation button (navButton).
Prevents the default anchor behavior.
Scrolls smoothly to the top of the corresponding section.

Section Highlighting:
activeSection: Highlights the section in the viewport and its corresponding navigation button.
Selects all navigation links (navActive).
Loops through each section and checks if it is in the viewport using getBoundingClientRect().
Adds the class your-active-class to the section and active_button to the corresponding navigation link if the section is in the viewport.
Removes these classes if the section is not in the viewport.

NavBar:
toggleNavBar: Shows the navigation bar while scrolling and hides it after 6 seconds of inactivity.
Sets the header style to be visible.
Clears any existing timeout.
Sets a timeout to hide the header after 6 seconds.

My script dynamically builds a navigation menu based on the sections of the webpage, adds smooth scrolling to section navigation, highlights the section and corresponding navigation link in the viewport, toggles the visibility of the navigation bar based on user scrolling activity, and includes a "Go Up" button to return to the top of the page.







