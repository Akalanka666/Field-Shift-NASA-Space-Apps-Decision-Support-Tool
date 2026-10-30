# Field-Shift-NASA-Space-Apps-Decision-Support-Tool#

<body>

<header>
        <div class="logo">🌿 Field Shift <span class="badge">NASA Data Powered</span></div>
        <nav>
            <a href="#tool">Explore Tool</a>
            <a href="https://www.spaceappschallenge.org/2026/challenges/adapting-farms-with-nasa-data/">About Challenge</a>
            <a href="file:///C:/Users/A/Desktop/map.html">About us</a>
        </nav>
    </header>
        
 <section class="hero">
        <div class="hero-badge">🚀 NASA International Space Apps Challenge Project</div>
        <h1>Field Shift: Adapting Farms with NASA Data</h1>
        <p>Empowering farmers with data-driven decision tools, utilizing NASA Earth observations (SMAP, ECOSTRESS, GPM) to model climate-resilient crop rotation strategies.</p>
    </section>

<div class="form-container" id="tool">
        <h2>පාරිසරික දත්ත පෝරමය (Environmental Data Form)</h2>

 <form action="process.php" method="POST">
            
<div class="form-group">
                <label for="date">Date:</label>
                <input type="date" id="date" name="date" required>
            </div>
<!-- Precipitation (mm) -->
            <div class="form-group">
                <label>Precipitation (mm):</label>
                <div class="input-row">
                    <input type="number" step="0.1" id="rainfall_1" name="rainfall[]" placeholder="Value 1" required>
                    <input type="number" step="0.1" id="rainfall_2" name="rainfall[]" placeholder="Value 2" required>
                    <input type="number" step="0.1" id="rainfall_3" name="rainfall[]" placeholder="Value 3" required>
                </div>
            </div>
 <!-- Soil Moisture (%) -->
            <div class="form-group">
                <label>Soil Moisture (%):</label>
                <div class="input-row">
                    <input type="number" step="0.1" id="soil_moisture_1" name="soil_moisture[]" min="0" max="100" placeholder="Value 1" required>
                    <input type="number" step="0.1" id="soil_moisture_2" name="soil_moisture[]" min="0" max="100" placeholder="Value 2" required>
                    <input type="number" step="0.1" id="soil_moisture_3" name="soil_moisture[]" min="0" max="100" placeholder="Value 3" required>
                </div>
            </div>
 <!-- Temperature (°C) -->
            <div class="form-group">
                <label>Temperature (°C):</label>
                <div class="input-row">
                    <input type="number" step="0.1" id="temp_1" name="temperature[]" placeholder="Value 1" required>
                    <input type="number" step="0.1" id="temp_2" name="temperature[]" placeholder="Value 2" required>
                    <input type="number" step="0.1" id="temp_3" name="temperature[]" placeholder="Value 3" required>
                </div>
            </div>

<div class="form-group">
                <label for="vegetation">Vegetation Level:</label>
                <select id="vegetation" name="vegetation" required>
                    <option value="">Select..</option>
                    <option value="dense">Dense (NDVI > 0.6)</option>
                    <option value="moderate">Moderate (NDVI 0.2 - 0.6)</option>
                    <option value="sparse">Sparse (NDVI < 0.2)</option>
                    <option value="none">Barren Land</option>
                </select>
            </div>

<div class="form-group">
                <label for="water_availability">Water Availability:</label>
                <select id="water_availability" name="water_availability" required>
                    <option value="">Select..</option>
                    <option value="high">High</option>
                    <option value="medium">Medium</option>
                    <option value="low">Low</option>
                </select>
            </div>

  <button type="submit" name="calculate">Calculate Average & Submit</button>
        </form>
    </div>
    
</body>
</html>
