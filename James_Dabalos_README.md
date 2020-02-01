Create a working day planner
    * Inside <div> container :
        * Add rows that will hold three columns
        * Three columns: hour block, description block, button
        * Add corresponding css class
        * Add id's to textareas that correspond to the same numerical value of buttons
    * Script - mainly using jquery
        * Add date and time
        * Display date and time
        * Create necessary variables
        * Create save button event handler
            * Grab value from button
            * Store as key (property)
            * Use the key to match the id of textarea to grab input
            * Store as description (value)
            * Create object {key,description}
            * Save in localstorage
        * Create a function that will loop through all description box
            * Color code them based on time
            * Render any saved descriptions using a function
        * Create rendering function
            * Run a check if localstorage is empty
                * Return if empty
                * Render if not
                    * Grab object from localstorage
                    * Use the index created from loop from before (since the call is nested inside the loop)
                    * Check if description is definded or not
                        * If undefined, do nothing
