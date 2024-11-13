<script>
        let currentPage = 1;
        let isLoading = false;

        // Function to fetch data from the server
        async function fetchData(page) {
            isLoading = true;
            const response = await fetch(`/data?page=${page}`);
            const data = await response.json();
            renderTableRows(data);
            isLoading = false;
        }

        // Function to render rows in the table
        function renderTableRows(data) {
            const tableBody = document.getElementById("table-body");
            data.forEach(row => {
                const tr = document.createElement("tr");
                tr.innerHTML = `
                    <td>${row.column1}</td>
                    <td>${row.column2}</td>
                    <td>${row.column3}</td>
                `;
                tableBody.appendChild(tr);
            });
        }

        // Load initial data
        fetchData(currentPage);

        // Function to handle infinite scrolling
        window.onscroll = function() {
            if (window.innerHeight + window.scrollY >= document.body.offsetHeight && !isLoading) {
                currentPage++;
                fetchData(currentPage);
            }
        };
    </script>
