# Amazon Label & Invoice Processor Pro

A lightning-fast, fully client-side web application designed for Amazon Sellers. This tool streamlines the fulfillment process by extracting, sorting, and formatting Amazon shipping labels and invoices into optimized PDFs for thermal printers and standard A4 paper.

## 🚀 Features

*   **Visual Page Manager:** Upload your raw Amazon PDF and visually review all pages. Click to delete any cancelled orders or extra pages before processing.
*   **Auto SKU Extraction:** Intelligently scans invoice pages and extracts the product SKU (based on the `(SKU) HSN` format) to help you organize your picking process.
*   **Drag-and-Drop Sorting:** Group and reorder your shipments by SKU. Keep similar items together to make warehouse picking significantly faster.
*   **Thermal Label Export (1x1):** Downloads a clean PDF containing *only* the shipping labels in your newly sorted order, perfectly formatted for a 4x6 thermal printer.
*   **Cut & Stack Invoice Export (2x2):** Downloads the invoices formatted in a mathematical 2x2 "Cut & Stack" grid. When you print and cut the stack into 4 quadrants, the invoices will remain in the exact sorted order!
*   **100% Private & Secure:** All PDF processing happens directly in your browser. No files are ever uploaded to a server or stored in a database.

## 🛠️ Technology Stack

*   **HTML5, CSS3, JavaScript (ES6)**
*   **[Tailwind CSS](https://tailwindcss.com/)** - For modern, responsive UI styling.
*   **[PDF.js](https://mozilla.github.io/pdf.js/)** - For rendering PDF thumbnails and extracting text.
*   **[pdf-lib](https://pdf-lib.js.org/)** - For modifying, splitting, and merging the final PDF documents.
*   **[SortableJS](https://sortablejs.github.io/Sortable/)** - For the smooth drag-and-drop SKU sorting interface.

## 📖 How to Use

1. **Upload:** Drag and drop your raw PDF file downloaded from Amazon (which contains alternating Labels and Invoices).
2. **Review:** Visually review the pages. Click any page to delete it (ensure your remaining page count is an even number so labels and invoices match up).
3. **Group & Sort:** Click "Group Orders". The app will read the text, extract the SKUs, and present them in a list. Drag and drop the rows to sort your batches.
4. **Download:** 
    * Click **Download Labels** to get your thermal printer file.
    * Click **Download Invoices** to get your A4 2x2 Cut & Stack file.

## 🌐 Hosting on GitHub Pages

This application requires no backend database or server. You can host it for free on GitHub Pages:

1. Create a new public repository on GitHub.
2. Upload the `index.html` file to the root of the repository.
3. Go to **Settings** > **Pages**.
4. Under **Source**, select `Deploy from a branch`.
5. Select the `main` branch and `/ (root)` folder, then click **Save**.
6. Within a minute, your app will be live at `https://<your-username>.github.io/<repository-name>/`.
