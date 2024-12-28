# Enzyme Backtracker

A simple web tool for estimating past enzyme levels based on current readings and enzyme half-lives. This tool can be useful in clinical settings to understand the potential timeline of enzyme changes.

## Description

This application allows users to input current levels of three common enzymes (AST, ALT, and LDH), along with the date and time the readings were taken. It then uses the enzymes' half-lives (default values are provided but are editable) to backtrack and estimate what the enzyme levels might have been at specified intervals in the past.

Key Features:
*   **Date and Time Input:**  Specify when the current enzyme levels were measured.
*   **Editable Half-Lives:**  Customize the half-lives of AST, ALT, and LDH, or use the default values.
*   **Custom Time Steps:** Control how many time steps to go back, and how large each step is.
*   **Transposed Table Output:**  View the historical enzyme estimates in a well organized table, with columns of Hours Ago, Date, Time, AST, ALT, and LDH
*   **Responsive Design:**  The tool is designed to be usable on various screen sizes.
*   **Collapsible Settings:** The default parameters for time and half life can be toggled.

## Usage

1.  **Clone the Repository:**
    ```bash
    git clone [YOUR_REPOSITORY_URL]
    ```

2.  **Open `main.html`:** Open the `main.html` file in your web browser.

3.  **Input Data:**
    *   Enter the current date and time of the enzyme measurement.
    *   Enter the current levels of AST, ALT, and LDH.
    *   Optionally, adjust the half-lives for each enzyme, the number of time steps to go back, and the time step size.

4.  **Calculate:** Click the "Calculate" button.

5.  **View Results:** The results will be displayed in a table below the form. The table will show estimated enzyme levels for timepoints going back from the specified current time.

## Input Parameters
* **Date/Time:** This specifies the date and time the user took their enzyme measurement.
* **AST Half-Life (hours, default 17):** The biological half-life of the Aspartate Aminotransferase (AST) enzyme.
* **ALT Half-Life (hours, default 72):** The biological half-life of the Alanine Aminotransferase (ALT) enzyme.
* **LDH Half-Life (hours, default 24):** The biological half-life of the Lactate Dehydrogenase (LDH) enzyme.
* **Time Steps (default 10):** The number of time points to calculate enzyme levels for.
* **Step Size (hours, default 12):** The amount of time between calculated time points.
* **Current AST Level:** The user's current AST level.
* **Current ALT Level:** The user's current ALT level.
* **Current LDH Level:** The user's current LDH level.

## Output Table Format
The table shows the following:
* **Time (h ago):** The number of hours in the past relative to current measurement.
* **Date:** The date of the estimated enzyme level.
* **Time:** The time of day of the estimated enzyme level.
* **AST:** The estimated AST enzyme level at the given timepoint.
* **ALT:** The estimated ALT enzyme level at the given timepoint.
* **LDH:** The estimated LDH enzyme level at the given timepoint.

## Example

If you enter the following:
* **Date/Time:** July 12 2024, 13:00
* **AST:** 100
* **ALT:** 200
* **LDH:** 300
* **AST Half-Life:** 17
* **ALT Half-Life:** 72
* **LDH Half-Life:** 24
* **Time Steps:** 3
* **Step Size:** 12

The program will produce an output table showing estimated enzyme values at three time points going back 12, 24, and 36 hours prior to 1:00PM on July 12.

## Technologies Used

*   HTML
*   CSS
*   JavaScript

## Contributing

Contributions are welcome! If you have any ideas for improvements, bug fixes, or new features, feel free to submit a pull request.

## License

[Add your license type here, if any (e.g., MIT License)]

## Issues

If you encounter any problems, please feel free to open an issue on the GitHub repository.

## Author
Mohammad Almeqdadi, MD
