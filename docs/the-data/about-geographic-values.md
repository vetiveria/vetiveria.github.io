---
layout: default
title: About Geographic Values
parent: The Data
nav_order: 2
---

# Buttons
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Decimals

This exercise is about hazardous waste in the states and territories of the U.S.A.  The locations of these facilities are encoded by the `fac_latitude` & `fac_longitude` fields.  However, a number of facilities do not have `fac_latitude` & `fac_longitude` values.  Hence, the latitude & longitude values of such facilities will be determined via `geopy`.  The decimal latitude & longitude values of

* https://enviro.epa.gov/enviro/EF_METADATA_HTML.tri_page?p_column_name=FAC_LATITUDE

* https://enviro.epa.gov/enviro/EF_METADATA_HTML.tri_page?p_column_name=FAC_LONGITUDE

are determined via the formula

$\qquad DD + \frac{MM}{60} + \frac{SS}{3600}$

<img src="https://render.githubusercontent.com/render/math?math={ \qquad \mathstrut{DD} %2B \mathstrut{\large{\frac{MM}{60}}} %2B \mathstrut{\large{\frac{SS}{3600}}} }"></img>

which converts DDMMSS coordinates to decimal form; note that each fac_latitude/fac_longitude is of the form DDMMSS.
