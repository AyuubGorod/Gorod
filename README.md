<!DOCTYPE html>
<html lang="so">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Diiwaangelinta Buugaagta</title>
    <style>
        /* CSS-kii hore ee qurxoon */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #f5f7fa, #c3cfe2);
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }
        .container {
            width: 90%;
            max-width: 800px;
            background: #fff;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            animation: fadeIn 1s ease-in-out;
        }
        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(-20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        h1 {
            text-align: center;
            background: linear-gradient(135deg, #16147c, #8a046d);
            color: #fffefe;
            font-size: 2.5em;
            margin-bottom: 20px;
            position: relative;
        }
        h1::after {
            content: '';
            width: 60px;
            height: 4px;
            background: #0a0458;
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            border-radius: 2px;
        }
        form {
            margin-bottom: 20px;
        }
        label {
            display: block;
            margin-bottom: 8px;
            font-weight: bold;
            color: #555;
        }
        input[type="text"], input[type="date"], select {
            width: 100%;
            padding: 12px;
            margin-bottom: 20px;
            border: 1px solid #ddd;
            border-radius: 8px;
            font-size: 16px;
            transition: border-color 0.3s ease, box-shadow 0.3s ease;
        }
        input[type="text"]:focus, input[type="date"]:focus, select:focus {
            border-color: #030b55;
            box-shadow: 0 0 8px rgba(40, 167, 69, 0.3);
            outline: none;
        }
        button {
            width: 100%;
            padding: 12px;
            background: linear-gradient(135deg, #16147c, #218838);
            color: #fff;
            border: none;
            border-radius: 8px;
            font-size: 16px;
            cursor: pointer;
            transition: background 0.3s ease, transform 0.3s ease;
        }
        button:hover {
            background: linear-gradient(135deg, #09076b, #1e7e34);
            transform: translateY(-2px);
        }
        button:active {
            transform: translateY(0);
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
            background: #fff;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        th, td {
            padding: 12px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }
        th {
            background: linear-gradient(135deg, #210a72, #218838);
            color: #fff;
            font-weight: bold;
        }
        tr:hover {
            background-color: #f1f1f1;
            transition: background-color 0.3s ease;
        }
        .footer {
            margin-top: 30px;
            text-align: center;
            font-size: 14px;
            color: #666;
            padding: 10px;
            background: #f8f9fa;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }
        .filter-section {
            margin-bottom: 20px;
            display: flex;
            gap: 10px;
        }
        .filter-section input, .filter-section select {
            flex: 1;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 8px;
            font-size: 16px;
            transition: border-color 0.3s ease, box-shadow 0.3s ease;
        }
        .filter-section input:focus, .filter-section select:focus {
            border-color: #28a745;
            box-shadow: 0 0 8px rgba(40, 167, 69, 0.3);
            outline: none;
        }
        .filter-section button {
            padding: 12px 20px;
            background: linear-gradient(135deg, #28a745, #051352);
            color: #fff;
            border: none;
            border-radius: 8px;
            font-size: 16px;
            cursor: pointer;
            transition: background 0.3s ease, transform 0.3s ease;
        }
        .filter-section button:hover {
            background: linear-gradient(135deg, #218838, #0f0352);
            transform: translateY(-2px);
        }
        .filter-section button:active {
            transform: translateY(0);
        }
    </style>
</head>
<body>

<div class="container">
    <h1>Hoyga Buugta Gorod</h1>
    
    <!-- Formka Diiwaangelinta -->
    <form id="bookForm">
        <label for="readerName">Magaca Aqriyaha:</label>
        <input type="text" id="readerName" name="readerName" required>
        
        <label for="bookName">Magaca Buuga:</label>
        <select id="bookName" name="bookName" required>
            <option value="adkeysi">1. Adkeysi</option>
            <option value="xeerka_ciqaabta_soomaaliyeed">2. Xeerka Ciqaabta Soomaaliyeed</option>
            <option value="muxamed_al_fatixi">3. Muxamed Al Fatixi</option>
            <option value="fakar_oo_hodan_noqo">4. Fakar oo Hodan Noqo</option>
            <option value="qab_iyo_quursi">5. Qab iyo Quursi</option>
            <option value="raad_raac_taarikhda_soomaaliyeed">6. Raad Raac Taarikhda Soomaaliyeed</option>
            <option value="sirdoon">7. Sirdoon</option>
            <option value="madxafka_cadaabka">8. Madxafka Cadaabka</option>
            <option value="basaasadi_ingiriska">9. Basaasadi Ingiriska</option>
            <option value="basaasadi_ingiriska"> 10. amiina al mufti         </option>
            <option value="basaasadi_ingiriska"> 11. s/ guud         </option>
            <option value="basaasadi_ingiriska">12. caadoyinka ilimaqabtay          </option>
            <option value="basaasadi_ingiriska">13. dagalka ranjariska          </option>
            <option value="basaasadi_ingiriska">14. sahayda sigasiga          </option>
            <option value="basaasadi_ingiriska">15. amiirka cas          </option>
            <option value="basaasadi_ingiriska">16. aabo hodan ah          </option>
            <option value="basaasadi_ingiriska">17. hawaale warran          </option>
            <option value="basaasadi_ingiriska">18. qamaamurinta musliminta          </option>
            <option value="basaasadi_ingiriska">19. soomaalida iyo soomaalinimada          </option>
            <option value="basaasadi_ingiriska">20. Aqris aayatin leh          </option>
            <option value="basaasadi_ingiriska">21. sirdoon 1aad          </option>
            <option value="basaasadi_ingiriska">22. sirdoon 2aad          </option>
            <option value="basaasadi_ingiriska">23. sirdoonka isra'iil          </option>
            <option value="basaasadi_ingiriska">24. kaalinta indheergaradka          </option>
            <option value="basaasadi_ingiriska">25. jiraalkay 1          </option>
            <option value="basaasadi_ingiriska">26. Loolan          </option>
            <option value="basaasadi_ingiriska">27. Dirkii sacamaallada          </option>
            <option value="basaasadi_ingiriska">28.  Jaceyl aan dhamat laheen          </option>
            <option value="basaasadi_ingiriska">29. power           </option>
            <option value="basaasadi_ingiriska">30. Dark psycholog 1aad          </option>
            <option value="basaasadi_ingiriska">31. Dark psycholog 2aad          </option>
            <option value="basaasadi_ingiriska">32. Dastuurka ku meel garka iyo fahamka arimaha sirdoonka           </option>

        </select>
        
        <label for="dateRead">Taariikhda La Aqriyay:</label>
        <input type="date" id="dateRead" name="dateRead" required>
        
        <label for="pagesRead">Inta Bogag La Aqriyay:</label>
        <input type="text" id="pagesRead" name="pagesRead" required>
        
        <button type="submit">Save</button>
    </form>

    <!-- Filter iyo Search Section -->
    <div class="filter-section">
        <input type="text" id="searchBook" placeholder="Raadi Buug...">
        <input type="date" id="filterDate">
        <button onclick="filterTable()">Filter</button>
    </div>

    <!-- Table-ka Xogta -->
    <table id="bookTable">
        <thead>
            <tr>
                <th>Magaca Aqriyaha</th>
                <th>Magaca Buuga</th>
                <th>Taariikhda La Aqriyay</th>
                <th>Inta Bogag La Aqriyay</th>
            </tr>
        </thead>
        <tbody>
            <!-- Xogta halkan waxaa lagu soo dari doonaa JavaScript -->
        </tbody>
    </table>

    <!-- Footer -->
    <div class="footer">
        <p>Diiwaangelinta Buugaagta &copy; 2023</p>
    </div>
</div>

<script>
    // JavaScript for saving data and filtering
    const bookForm = document.getElementById('bookForm');
    const bookTable = document.getElementById('bookTable').getElementsByTagName('tbody')[0];

    // Function to save data to localStorage
    function saveToLocalStorage(data) {
        let books = JSON.parse(localStorage.getItem('books')) || [];
        books.push(data);
        localStorage.setItem('books', JSON.stringify(books));
    }

    // Function to load data from localStorage
    function loadFromLocalStorage() {
        const books = JSON.parse(localStorage.getItem('books')) || [];
        books.forEach(book => {
            const newRow = bookTable.insertRow();
            newRow.insertCell(0).textContent = book.readerName;
            newRow.insertCell(1).textContent = book.bookName;
            newRow.insertCell(2).textContent = book.dateRead;
            newRow.insertCell(3).textContent = book.pagesRead;
        });
    }

    // Load data when the page is loaded
    window.addEventListener('load', loadFromLocalStorage);

    // Save data when the form is submitted
    bookForm.addEventListener('submit', function(event) {
        event.preventDefault();
        
        const readerName = document.getElementById('readerName').value;
        const bookName = document.getElementById('bookName').value;
        const dateRead = document.getElementById('dateRead').value;
        const pagesRead = document.getElementById('pagesRead').value;
        
        const newRow = bookTable.insertRow();
        newRow.insertCell(0).textContent = readerName;
        newRow.insertCell(1).textContent = bookName;
        newRow.insertCell(2).textContent = dateRead;
        newRow.insertCell(3).textContent = pagesRead;
        
        // Save data to localStorage
        saveToLocalStorage({ readerName, bookName, dateRead, pagesRead });
        
        // Clear form
        bookForm.reset();
    });

    // Filter function
    function filterTable() {
        const searchBook = document.getElementById('searchBook').value.toLowerCase();
        const filterDate = document.getElementById('filterDate').value;
        const rows = bookTable.getElementsByTagName('tr');
        
        for (let i = 1; i < rows.length; i++) { // Start from 1 to skip header
            const bookName = rows[i].getElementsByTagName('td')[1].textContent.toLowerCase();
            const dateRead = rows[i].getElementsByTagName('td')[2].textContent;
            
            if ((bookName.includes(searchBook) || searchBook === '') && (dateRead === filterDate || filterDate === '')) {
                rows[i].style.display = '';
            } else {
                rows[i].style.display = 'none';
            }
        }
    }
</script>

</body>
</html>
