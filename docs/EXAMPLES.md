# `UrbanMapper`’s Examples Playground

!!! warning "New here? Start with the basics!"
    Before jumping into this playground, make sure you’ve  walked through
    the [Getting Started Step-By-Step](./getting-started/quick-start_step_by_step.md)
    and [Getting Started W/ Pipeline](./getting-started/quick-start_pipeline.md) guides. They’re explaining quite in depth `UrbanMapper`—trust us,
    it could be useful before delving into these examples, which are more straightforward and focused on specific tasks.

Welcome to the `examples/` folder, where you will get hands-on experience with `UrbanMapper`!  This set of Jupyter
notebooks guides users through the process of loading, mapping, enhancing, and visualising urban data. These examples
are suitable for both newcomers to urban analysis and experienced urban planners seeking to improve their process. 

Explore the full potential of `UrbanMapper` with these real-world demos, including Brooklyn collisions, Paris trees, cab rides,
to name a few.

!!! tip "Where’s the data at?"
    All the datasets powering these examples are public and ready for you to grab. Pick your channel:

    - **Channel 1: Straight from the source**
        - Check the links in each notebook, download from the official sites, and drop them into your `data/` folder.
    - **Channel 2: HuggingFace OSCUR datasets hub**
        - If you prefer HuggingFace, you can find the datasets in the [OSCUR datasets hub](https://huggingface.co/datasets/oscur).
            Use the `datasets` library to load them directly into your code (integrated with `UrbanMapper`):
            ```python
            import urbanmapper as um
            loader = um.UrbanMapper().loader.from_huggingface("oscur/pluto") # replace "pluto" with the dataset you want.
            gdf = loader.load()
            print(gdf.head()) 
            ```

## Execution Status at a Glance

!!! info "A quick heads-up on execution"
    Notebooks are either executed in the docs or kept as static previews. If you want the full interactive experience,
    run them locally from the `examples/` folder in the repository.

=== "▶️ Executed in docs"

    **2-End-to-End**

    - [Pipeline Way](../copy_of_examples/2-End-to-End/2-pipeline_way)

=== "🧊 Not executed in docs"
    These render as static previews. Run locally for full outputs.

    **1-Per-Module**

    - [Loader](../copy_of_examples/1-Per-Module/1-loader)
    - [Urban Layer](../copy_of_examples/1-Per-Module/2-urban_layer)
    - [Imputer](../copy_of_examples/1-Per-Module/3-imputer)
    - [Filter](../copy_of_examples/1-Per-Module/4-filter)
    - [Enricher](../copy_of_examples/1-Per-Module/5-enricher)
    - [Visualiser](../copy_of_examples/1-Per-Module/6-visualiser)
    - [urban pipeline](../copy_of_examples/1-Per-Module/7-urban_pipeline)
    - [Pipeline Generator](../copy_of_examples/1-Per-Module/8-pipeline_generator)

    **2-End-to-End**
    - [Step by Step](../copy_of_examples/2-End-to-End/1-step_by_step)

    **3-Case-Studies**

    - [Downtown BK Collisions - Step by Step](../copy_of_examples/3-Case-Studies/1-Downtown-BK-Collisions/1-Downtown_BK_Collisions_StepByStep)
    - [Downtown BK Collisions - Pipeline](../copy_of_examples/3-Case-Studies/1-Downtown-BK-Collisions/2-Downtown_BK_Collisions_Pipeline)
    - [Downtown BK Collisions - Advanced Pipeline](../copy_of_examples/3-Case-Studies/1-Downtown-BK-Collisions/3-Downtown_BK_Collisions_Advanced_Pipeline)
    - [Downtown BK Collisions - Advanced Pipeline Extras](../copy_of_examples/3-Case-Studies/1-Downtown-BK-Collisions/4-Downtown_BK_Collisions_Advanced_Pipeline_Extras)
    - [Downtown BK Taxi Trips - Step by Step](../copy_of_examples/3-Case-Studies/2-Downtown-BK-Taxi-Trips/1-Downtown_BK_Taxi_Trips_StepByStep)
    - [Downtown BK Taxi Trips - Pipeline](../copy_of_examples/3-Case-Studies/2-Downtown-BK-Taxi-Trips/2-Downtown_BK_Taxi_Trips_Pipeline)
    - [Downtown BK Taxi Trips - Advanced Pipeline](../copy_of_examples/3-Case-Studies/2-Downtown-BK-Taxi-Trips/3-Downtown_BK_Taxi_Trips_Advanced_Pipeline)
    - [Downtown BK Taxi Trips - Advanced Pipeline Extras](../copy_of_examples/3-Case-Studies/2-Downtown-BK-Taxi-Trips/4-Downtown_BK_Taxi_Trips_Advanced_Pipeline_Extras)
    - [EU Restaurants Pipeline](../copy_of_examples/3-Case-Studies/3-Europe-Restaurants/1-EU_Restaurants_Pipeline)
    - [Paris Remarkable Trees - Pipeline](../copy_of_examples/3-Case-Studies/4-Paris-Remarkable-Trees/1-Paris_Remarquable_Trees_Pipeline)
    - [Paris Remarkable Trees - Advanced Pipeline](../copy_of_examples/3-Case-Studies/4-Paris-Remarkable-Trees/2-Paris_Remarquable_Trees_Advanced_Pipeline)
    - [Overture Pipeline](../copy_of_examples/3-Case-Studies/5-Overture-instead-of-OSM/1-overture_pipeline)
    - [Advanced Overture Pipeline](../copy_of_examples/3-Case-Studies/5-Overture-instead-of-OSM/2-overture_pipeline_advanced)

    **4-External-Libraries-Usages**

    - [Auctus Search](../copy_of_examples/4-External-Libraries-Usages/1-auctus_search)
    - [Interactive Table VIS](../copy_of_examples/4-External-Libraries-Usages/2-interactive_table_vis)
    - [Jupyter GIS Multi Pipeline - One Pipeline](../copy_of_examples/4-External-Libraries-Usages/3-jupyter_gis_multi_pipeline/1-one_pipeline)
    - [Jupyter GIS Multi Pipeline - Two Pipeline](../copy_of_examples/4-External-Libraries-Usages/3-jupyter_gis_multi_pipeline/2-two_pipeline)
    - [Jupyter GIS Multi Pipeline - Three Pipeline](../copy_of_examples/4-External-Libraries-Usages/3-jupyter_gis_multi_pipeline/3-three_pipeline)

!!! tip "Want the full interactive experience?"
    Clone the repo, pull the datasets, and run any notebook locally from `examples/`. Most notebooks contain links to
    their data sources or instructions in the first few cells.
