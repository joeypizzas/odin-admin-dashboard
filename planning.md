# Planning for odin admin dashboard

Grid architecture:
- Top level grid container with two columns and two rows. Column 2 is ~4x column 1. Row 2 is ~5x Row 1. Sidebar is column 1 and rows 1-2. Header is column 2, row 2. Body is column 2, row 2. Maybe don't need to expicitly set rows?
    - Sidebar: 3 divs. One for each section. Grid. Gap between sections. Align content near the start (top). 
        - Each section underneath starts with columns insetad of rows with grid. Gap between icon and title. Justify content near start (left). 
    - Header: One column, two rows. Grid. Gap between tows, maybe? Set paddin top/bottom, left/right. 
        - Top row header. Grid. Two columns, one row. Gap or Space between?  
            - Top row left column. Two items, two columns, space between? 
            - Top row right column, three items, three columns, space between? 
        - Bottom row header. Grid. Two columns, one row. Space between. 
            - Bottom row left. Two items, two columns, grid. Space between. 
                - Right column has grid with two rows. Top text size is way bigger than bottom. top justify item is start. 
            - Bottom row right. Three items, three columns, grid, space between. 
    - Body: Grid. 2 columns, 2 rows. column 1 is 3 times bigger than column 2. Row 2 is 7-8x bigger than row 1. 
        - Column 1, row 1: header, justify-item to left. 
        - Column 2, row 1: header: justify item to left. 
        - Column 1, row 2: auto-fit columns to wrap with grid. Gap. 
            - Cards inside: Coloring on left of div? Two rows. Header/body and icons. Top has justify-item start, bottom, justify-item end. 
                Two row grid for body and header with smaller gap. 
        Column 2, row 2: two rows. Top is just card. Bottom is card and header. Grid. Gap. 
            - Top row: Card, three items, grid. Bottom two have border. Padding inside container. 
                - Grid in each item with header and content. Justify item start. 
            - Bottom row: two items. Grid. Bottom item 5-6x larger. 
                - Header: justify item start. 
                - Card, 4 items, grid. Padding and space between. 
                    - Rows: Grid with two items each, grid starting with columns. Gap and justify content start. 
                        - Images as is. 
                        - Grid with two rows for header and sub-header. Justify item start. 