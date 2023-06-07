---
title: murine-source
schema_name: murine-source
category: Other TSVs
all_versions_deprecated: False
exclude_from_index: False
layout: default
---

Related files:

- [📝 Excel template](https://raw.githubusercontent.com/hubmapconsortium/ingest-validation-tools/main/docs/murine-source/murine-source.xlsx): For metadata entry.
- [📝 TSV template](https://raw.githubusercontent.com/hubmapconsortium/ingest-validation-tools/main/docs/murine-source/murine-source.tsv): Alternative for metadata entry.







## Metadata schema

### Field types
- *Boolean* fields can be given as `TRUE`/`FALSE`, `True`/`False`, `true`/`false`, or `1`/`0`.  


<details markdown="1" open="true"><summary><b>Version 0 (current)</b></summary>

<blockquote markdown="1">

[`local_lifespan_data`](#local_lifespan_data)<br>
[`room_health_status`](#room_health_status)<br>
[`room_temperature`](#room_temperature)<br>
[`rack_setup`](#rack_setup)<br>
[`light_cycle`](#light_cycle)<br>
[`bedding`](#bedding)<br>
[`diet`](#diet)<br>
[`water_source`](#water_source)<br>
[`cage_enhancements`](#cage_enhancements)<br>

</blockquote>

<a name="local_lifespan_data"></a>
##### [`local_lifespan_data`](#local_lifespan_data)
A free text description of how long mice live within the local environment. It is recommended to provide the median or maximum values for murine lifespans. Leave blank if not applicable.

| constraint | value |
| --- | --- |
| required | `False` |

<a name="room_health_status"></a>
##### [`room_health_status`](#room_health_status)
A description of the pathogen and opportunist exclusion level of the room where the source is housed. Leave blank if not applicable.

| constraint | value |
| --- | --- |
| required | `False` |
| enum | `Pathogen free`, `Pathogen and opportunist free`, or `Other` |

<a name="room_temperature"></a>
##### [`room_temperature`](#room_temperature)
The temperature value in Celsius of the room where the source is housed. An example is "23". Leave blank if not applicable.

| constraint | value |
| --- | --- |
| type | `number` |
| required | `False` |

<a name="rack_setup"></a>
##### [`rack_setup`](#rack_setup)
The rack setup type in which the source is housed. Leave blank if not applicable.

| constraint | value |
| --- | --- |
| required | `False` |
| enum | `Biocontainment`, `Ventilated`, `Micro-Isolator`, or `Conventional` |

<a name="light_cycle"></a>
##### [`light_cycle`](#light_cycle)
The light cycle in the room where the source is housed. "Standard/default" refers to 12-hour photoperiods (e.g., lights on at 7:00 AM, lights off at 7:00 PM). "Longer photoperiods" refers to 14-hour photoperiods (e.g., lights on at 7:00 AM, lights off at 9:00 PM). "Reverse lightcycles" means that the the timing of the 12-hour photoperiod is reversed (.e.g, lights on at 7:00 PM, lights off at 7:00 AM). Leave blank if not applicable.

| constraint | value |
| --- | --- |
| required | `False` |
| enum | `Standard/default`, `Longer photoperiods`, or `Reverse light cycles` |

<a name="bedding"></a>
##### [`bedding`](#bedding)
The type of cage bedding in the cage where the source is housed. Leave blank if not applicable.

| constraint | value |
| --- | --- |
| required | `False` |
| enum | `Aspen chip`, `Aspen shaving`, `Pine chip`, `Pine shaving`, `1/4-inch corncob`, `1/4-inch pelleted cellulose`, `Refined virgin diced cellulose`, `Non-contact cage board`, `Wire mesh`, or `Other` |

<a name="diet"></a>
##### [`diet`](#diet)
A free text description of the source's diet.

| constraint | value |
| --- | --- |
| required | `True` |

<a name="water_source"></a>
##### [`water_source`](#water_source)
A free text description of the source's water supply, including any treatments to the water. Leave blank if not applicable.

| constraint | value |
| --- | --- |
| required | `False` |

<a name="cage_enhancements"></a>
##### [`cage_enhancements`](#cage_enhancements)
Environmental enrichments present in the source’s cage. Leave blank if not applicable.

| constraint | value |
| --- | --- |
| required | `False` |
| enum | `Nestlets`, `Nest boxes/shelters`, `Shelter tubes`, `Wooden chew sticks`, `Nylon bones`, or `Other` |

</details>

