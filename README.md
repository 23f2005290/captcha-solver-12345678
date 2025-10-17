# Simple Captcha Solver UI

This project provides a straightforward, single-file web application to display and interact with captcha images. It's designed to be responsive and uses Tailwind CSS for styling. Users can load captcha images either from a default local file or by providing a URL parameter, and then attempt to solve them by entering the perceived text.

## Features

*   **Responsive Design**: Built with Tailwind CSS, ensuring a good user experience across various device sizes.
*   **Dynamic Image Loading**: Loads `sample.png` by default, or an external image if a `url` query parameter is provided.
*   **Captcha Input Field**: A dedicated input area for users to type their captcha solution.
*   **Client-Side Feedback**: Provides immediate feedback on whether the entered text matches the expected solution (for `sample.png`). For external images, it acknowledges the input.

## How to Use

1.  **Open `index.html`**: Simply open the `index.html` file in your web browser.
2.  **Default Captcha**: The application will display `sample.png` by default. Try entering "ADUR3" to see the "Correct" message.
3.  **Load Custom Captcha Image**: To load an external captcha image, append a `?url=` query parameter to your browser's address bar, followed by the URL of the image.

    *Example:*
    `file:///path/to/your/index.html?url=https://example.com/path/to/your/captcha.png`
    (Note: Replace `file:///path/to/your/index.html` with the actual path to your file, or host it on a web server.)

    *Example (if hosted):*
    `https://your-domain.com/index.html?url=https://example.com/another-captcha.jpg`

4.  **Enter Solution**: Type the characters you see in the captcha image into the input field.
5.  **Verify**: Click the "Verify Captcha" button to check your solution.

## Technologies Used

*   **HTML5**: Structure of the web page.
*   **Tailwind CSS**: Utility-first CSS framework for styling and responsiveness.
*   **JavaScript**: For dynamic image loading and client-side interaction logic.

## Project Structure

*   `index.html`: The main and only HTML file containing the entire application.
*   `sample.png`: The default captcha image.
*   `README.md`: This file.
*   `LICENSE`: The MIT License for this project.

## Important Note on Solver Functionality

This application provides a *user interface* for a human to solve captchas. For `sample.png`, it includes a hardcoded correct answer ("ADUR3") for demonstration. For external images loaded via URL, the client-side JavaScript can only acknowledge your input. A true automated captcha solver or robust verification for arbitrary images would require advanced image processing (OCR) and server-side logic, which is beyond the scope of this single-file frontend demonstration.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.