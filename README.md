# AME-373-Vehicle-Dynamics-_Algorithmic-thinking-with-python-
This will be the repo with all the codes from the labs
This repo holds the code for the Python labs I run alongside AME 373 Vehicle Dynamics. Each lab is a small model of a topic we cover in class, built from *Automotive Chassis Engineering*. I want you to run the code, change the numbers, and see what happens to the vehicle.

## Books

- David Barton & John D. Fieldhouse, *Automotive Chassis Engineering*, 2nd Ed.
- Stuart Macey & Geoff Wardle, *H Point: The Fundamentals of Car Design & Packaging*

Read the matching chapter before each lab. I follow the book's notation in the code.

## Labs

| Lab | Date | Topic | Folder |
|-----|------|-------|--------|
| 01 | Nov 2 | Setup, tractive force and tractive resistance | `labs/01_tractive_force` |
| 02 | Nov 9 | Load transfer, straight-line motion | `labs/02_load_transfer_straight` |
| 03 | Nov 16 | Load transfer during cornering | `labs/03_load_transfer_cornering` |
| 04 | Nov 23 | Braking kinetics, brake proportioning, adhesion utilisation | `labs/04_braking` |
| 05 | Nov 30 | Wheel/axle locking, pitch under braking, ABS | `labs/05_lock_pitch_abs` |
| 06 | Dec 7 | Springs, dampers, suspension kinematics, roll centres | `labs/06_suspension` |

We will follow the AME 373 schedule.

## Setup

```bash
git clone https://github.com/<your-username>/vehicle-dynamics-python.git
cd vehicle-dynamics-python
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter lab
```

`requirements.txt`:

```
numpy
scipy
matplotlib
pandas
jupyterlab
```

Run `git pull` before each lab to get the new folder.

## Running a lab

```bash
cd labs/01_tractive_force
python model.py
```

You can also open `lab.ipynb` in Jupyter Lab.

## Conventions

- SI units throughout (m, kg, N, s, rad)
- x forward, y left, z up (SAE axes)
- Vehicle parameters are read from `data/*.json`
- Each lab has one `model.py` with a `__main__` block that runs the example

## Where this is going

- [x] Repo setup
- [ ] Labs 01 to 06
- [ ] A full-vehicle model that combines all the labs

## Questions and fixes

If you find a mistake in the code or a lab that doesn't run, open an issue. If you have a fix, work on a branch named after the lab (for example `lab-03-cornering`) and open a pull request.

## License

MIT
