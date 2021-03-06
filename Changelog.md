
# V 0.24.2
## Added features:
--

## Fixed bugs:
--

## Enhancements:
1. Enhanced precision by created DMX-Profiles.
2. In case of an invalid user input, an error message is displayed.

---

# V 0.24.1
## Added features:
--

## Fixed bugs:
1. Invalid Executornumber 'PAGE'.00 is chosen when all Executors on the chosen page are taken.
    FIXED.
2. Invalid Executornumber 'PAGE'.0.01 is chosen when all Executors on the chosen page are taken
   and the preferred executor number were entered without an page (e.g. "10" instead of "1.10")
   FIXED.

## Enhancements:
1. CSContainer can be moved to any executor.
2. Using CSF names twice is prevented by requesting user to enter the CSF name
   until the chosen name is not already in use.
3. The CSFader now gets labeled according to the scheme "[CSF Name] CSF".

---

# V 0.24.0
## Added features:
1. CSContainer is now assigned to an executor, to enable executor options.
    - The system variable $CSC_[CSF NAME] is added which contains the executor number of the CSContainer. 
      If CSContainer is moved, it has to be updated.

## Fixed bugs:
--

## Enhancements:
1. CSFader is now swop protected.
2. "React To Master" is disabled for CSFixtures

---

# V 0.23.7
## Added features:
--

## Fixed bugs:
--

## Enhancements:
1. Performance enhancements through code optimizations.

---

# V 0.23.6
## Added features:
--

## Fixed bugs:
1. When running CSF more then one time, CSLayer gets recreated and overwritten every time.
    Fixed.
    Changings for the User:
    1.1. The second CSFixture is appended to the existing Layer and the existing Universe.
    1.2. Added GrandMA2 show variables $CSF_ADDR_CACHE and $CSF_UNI to enable patching and using multiple CSFixtures.
         These variables shall not be changed by the user.
2. When "1.10" is entered as executor number, it gets misinterpreted as "1.1"
    Fixed.
3. Finding an alternative executor fails sometimes and leads to a plugin crash.
    Fixed.


## Enhancements:
1. DMX Profiles can now be associated with the mode and the fixture version they were created with. 
   Schema is "CSF_Profile [INDEX]/[STEPS]_[VERSION]" (without []).
2. Performace enhancements through code optimizations.
