<p align="center">
 <img width="100px" src="logo.svg" align="center" alt="Logo" />
 <h2 align="center">CBED</h2>
 <h3 align="center">Database for Building Energy in China</h3>
 <p align="center">A FAIR Framework for Transparent, Secure Sharing of Chinese Building Energy-Efficient Design Datasets</p>
</p>
<p align="center">
  <a href="https://buildingdata.xauat.edu.cn/"><img alt="buildingdata" src="https://img.shields.io/badge/CBED Platform-063c7c?style=flat&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABQAAAAUCAYAAACNiR0NAAAACXBIWXMAAAsTAAALEwEAmpwYAAABQ0lEQVQ4jZ3UPU8UURjF8d8ubwmhopGAQKSDymhjQWm30hEbwkthgV9AQkUJFq5+AyVsIYXfwspADRWSYAMfgIIQH4qdjZv1zp1lT3Izd86c88/cZJ6pRYQ+9BY1HFcmI6JqvYl/WqnKV8Ga8b+agwCfRcRpAtbRaUQs9AvcyIB6tVkF/PYIWEeHKeCLiLgYANbR74JBRGxXhP9ExExEzEbEVUX2fR0rma/qEk/xCg3M4jyTbwzjOhNYwBpaxf0cFlE2DTf1DOxzUWx1ebuYLq4p1XLAA6wm/H18Len8zQFv8DrhL2u/+X3i2V0OCGMJ7x4j2j+LXmWPPIFfCf8E4xhKlXLALRwm/D08LyvlgJ9wi6Mev4GdQYCj+IgNnHX5X/CyrFPHkwz0A9axhO+ZXEdTw/ihfFrGMVns32mP3XwG+PMBYdAQPwkBdngAAAAASUVORK5CYII=&logoColor=white" /></a>
  <a href="https://github.com/buildingdata"><img alt="Github" src="https://img.shields.io/badge/GitHub-100000?style=flat&logo=github&logoColor=white" /></a>
  <a href="https://github.com/buildingdata/CBED-portal/blob/master/LICENSE"><img alt="License" src="https://img.shields.io/github/license/buildingdata/CBED-portal.svg?style=flat" /></a>
  <a href="https://github.com/buildingdata/CBED-portal/releases"><img src="https://img.shields.io/github/v/release/buildingdata/CBED-portal?label=version&style=flat" /></a>
  <a href="https://doi.org/10.5281/zenodo.14562142"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.14562142.svg" /></a>
</p>

### Abstract

The publication and platform-based dissemination of building energy-efficient design data are essential for advancing green building and energy conservation. Supported by China’s Ministry of Science and Technology, this initiative meets the pressing demand for standardized, accessible datasets to inform sustainable architectural practices. Key datasets—including building climate dataset, thermal and HVAC design conditions dataset, building energy simulation weather year dataset, and occupant thermal comfort indices dataset—require high-resolution meteorological and behavioral data, along with complex modeling. However, access is often restricted by national policy and privacy constraints. The CBED platform addresses these challenges by integrating building science methodologies with FAIR (Findable, Accessible, Interoperable, Reusable) principles to ensure transparency and interoperability. Its architecture employs automated data engineering workflows via the SSM framework, with built-in quality assurance and SSL/TLS encryption for security. By aligning domain-specific computation with FAIR-compliant governance, CBED offers a reproducible model for global collaboration, enabling researchers to access and contribute high-quality datasets and accelerating innovation in sustainable building technologies. 

### Repository

The database files are located in the `/sql` directory, and the open source code for the site is in the `/web` directory, which has the following directory structure.

```
/sql
/web
├── /frontend        # front-end
├── /app_front       # mobile-app
└── /backend         # back-end
```

### Installation

#### 1. Clone

Clone this repository and sql import the data tables to mysql:

```bash
git clone https://github.com/buildingdata/CBED-portal.git
```

#### 2. Download dependencies

Navigate to the `/web/backend` project directory and run it:

```bash
mvn clean install
```

This will download all required dependencies and compile the project.

#### 3. Run project

Run the application using the following command:

```bash
mvn spring-boot:run
```

This will start the embedded server (usually Tomcat).

#### 4. View

Once the server is up, open your browser and go to:

```bash
http://localhost:8080
```

### Open data

This code repository is shared for [scientific data](https://www.nature.com/sdata/).

 <img width="150px" src="scidata.svg" align="right" alt="Logo" />

### License

The code is available under the [GPL-3.0 license](https://github.com/buildingdata/CBED-portal/blob/master/LICENSE)
