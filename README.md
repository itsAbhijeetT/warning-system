# HYDRO-NOWCAST | Urban Flood Nowcasting System
### Smart India Hackathon 2026 — MoES / NCMRWF (Disaster Management & Software)

An operational, real-time **Coupled Drainage–Rainfall Urban Flood Nowcasting and Safe Emergency Routing Platform** with street-level resolution.

---

## Key Features

1. **True Two-Way Coupling (Surface ↔ Drainage)**:
   Overland water enters storm drains; when downstream pipes choke ($HGL > \text{ground}$), water surcharges and erupts back onto street surfaces.
2. **Sub-Second 2D Cellular Automata Routing**:
   Vectorized diffusive-wave routing over high-resolution DEM grids that completes 3-hour predictions in sub-seconds.
3. **Data-Sparse Drainage Auto-Inference**:
   Automatically infers hydraulic drainage graphs from road topography and DEM slope for ULBs with missing GIS data.
4. **Flood-Safe Dynamic Navigation (Module E)**:
   Dynamic A* routing penalizing submerged roads with vehicle clearance thresholds (Ambulances at 35 cm vs Civilians at 15 cm).
5. **Historical Backtesting Engine**:
   Pre-loaded with verified historical deluges (Mumbai 2005 / Chennai 2015) benchmarked with Critical Success Index (CSI) and confusion matrices.
6. **ULB Drain Calibration Tool**:
   Allows municipal engineers to interactively resize bottleneck conduits and test "what-if" flood alleviation works.

---

## Quick Start

### 1. Requirements
- Python 3.10+ (tested on Python 3.14)
- Packages: `fastapi`, `uvicorn`, `numpy`, `scipy`

### 2. Launch System
```powershell
python run_system.py
```

### 3. Open Command Center
Open your browser and navigate to:
```
http://localhost:8000/
```
