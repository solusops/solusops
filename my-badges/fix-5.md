<img src="https://my-badges.github.io/my-badges/fix-5.png" alt="I did 5 sequential fixes." title="I did 5 sequential fixes." width="128">
<strong>I did 5 sequential fixes.</strong>
<br><br>

Commits:

- <a href="https://github.com/OpenDistricts/Open-Districts/commit/bebeb5af5d4a916a256f23cf330e707ddb866bfe">bebeb5a</a>: Fix: Create missing vellore.geojson for Tamil Nadu district

Vellore district was missing its geojson file, causing map fallback to generic grid.
Created vellore.geojson with 5 tehsil subdivisions.
- <a href="https://github.com/OpenDistricts/Open-Districts/commit/7cd5ca7f085d4ce8e106594050ad8890d1cee1ed">7cd5ca7</a>: Fix: Create missing raipur.geojson for Chhattisgarh district

Raipur district was showing greyed out because its geojson file didn't exist.
This caused map fallback to mock grid (generic squares) instead of actual geometry.

Created raipur.geojson with 5 tehsil subdivisions:
- raipur (Raipur City) - center-south
- naya-raipur (Naya Raipur) - east
- tilda-neora (Tilda Neora) - north
- abhanpur (Abhanpur) - west
- arany (Arang) - south

Events can now render to correct regionIds instead of appearing greyed out.
- <a href="https://github.com/OpenDistricts/Open-Districts/commit/4d74665eeb23007e24987369502daf520326a02a">4d74665</a>: Fix: Remove duplicate dataPoints for Gurugram (5 was overriding 20)
- <a href="https://github.com/OpenDistricts/Open-Districts/commit/597d69e6141a91d8156fbb4c53934aa6cee04993">597d69e</a>: Fix: Correct all district bounds to match actual geometry (fixes map navigation)

11 districts had incorrect bounding boxes that didn't match their actual geojson geometry.
This caused map fitBounds to center on wrong locations, sending users out of map area.

Fixed districts:
- HR Gurugram: Extended east bounds to 77.22 (was 76.84)
- GJ Surat: Extended south bounds to 20.82 (was 21.20)
- MH Pune: Extended south bounds to 17.89 (was 19.00)
- OD Khordha: Extended south/east bounds
- BR Gaya: Extended south bounds
- RJ Jaipur: Extended south bounds
- PB Jalandhar: Extended north/east bounds
- MP Ujjain: Extended south bounds
- UP Sitapur: Extended north/east bounds
- KA Mysuru: Extended south/east bounds
- WB Hugli: Extended south/east bounds

All bounds now precisely match actual rendered geometry.
- <a href="https://github.com/OpenDistricts/Open-Districts/commit/13996b80c0011fe604564cbc5adc2b97ad72a3b5">13996b8</a>: Fix: Add dataPoints field to all mock districts


Created by <a href="https://github.com/my-badges/my-badges">My Badges</a>