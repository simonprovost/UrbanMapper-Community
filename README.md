<div align="center">
   <h1>UrbanMapper Community</h1>
   <h3>Enrich Urban Layers Given Urban Datasets</h3>
   <p><i>with ease-of-use API and Sklearn-alike Shareable & Reproducible Urban Pipeline</i></p>
   <p>
      <img src="https://img.shields.io/pypi/v/urban-mapper-community?label=Version&style=for-the-badge" alt="PyPI Version">
      <img src="https://img.shields.io/static/v1?label=Beartype&message=compliant&color=4CAF50&style=for-the-badge&logo=https://avatars.githubusercontent.com/u/63089855?s=48&v=4&logoColor=white" alt="Beartype compliant">
      <img src="https://img.shields.io/static/v1?label=UV&message=compliant&color=2196F3&style=for-the-badge&logo=UV&logoColor=white" alt="UV compliant">
      <img src="https://img.shields.io/static/v1?label=RUFF&message=compliant&color=9C27B0&style=for-the-badge&logo=RUFF&logoColor=white" alt="RUFF compliant">
      <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter">
      <img src="https://img.shields.io/static/v1?label=Python&message=3.10%2B&color=3776AB&style=for-the-badge&logo=python&logoColor=white" alt="Python 3.10+">
      <img src="https://img.shields.io/github/actions/workflow/status/simonprovost/UrbanMapper-Community/compile.yaml?style=for-the-badge&label=Compilation&logo=githubactions&logoColor=white" alt="Compilation Status">
   </p>
</div>



![UrbanMapper Cover](https://i.imgur.com/axoY0qm.jpeg)


___

## UrbanMapper & Urban Mapper Community, In a Nutshell

`UrbanMapper` lets you link your data to spatial features—matching, for example, traffic events to streets—to enrich
each location with meaningful, location-based information. Formally, it defines a spatial enrichment
function $f(X, Y) = X \bowtie Y$, where $X$ represents urban layers (e.g., `Streets`, `Sidewalks`, `Intersections` and
more)
and $Y$ is a user-provided dataset (e.g., `traffic events`, `sensor data`). The operator $\bowtie$ performs a spatial
join, enriching each feature in $X$ with relevant attributes from $Y$.

In short, `UrbanMapper` is a Python toolkit that enriches typically plain urban layers with datasets in a reproducible,
shareable, and easily updatable way using minimal code. For example, given `traffic accident` data and a `streets` layer
from [OpenStreetMap](https://www.openstreetmap.org), you can compute accidents per street with
a [Scikit-Learn](https://scikit-learn.org/stable/)–style pipeline called the `Urban Pipeline`—in under 15 lines of code.
As your data evolves or team members want new analyses, you can share and update the `Urban Pipeline` like a trained
model, enabling others to run or extend the same workflow without rewriting code.

**About the community-fork**: please scroll-down to the #Acknowledgments section below to learn more about the history of the project.

## Installation

Install `UrbanMapper-Community`:

 ```bash
 uv add urban-mapper-community
 # pip install works too!
 ```

Then launch Jupyter Lab to explore `UrbanMapper`:

```bash
uv run jupyter lab
```

# Getting Started with UrbanMapper

We highly recommend exploring the [UrbanMapper Documentation](https://urbanmapper.readthedocs.io/en/latest/), starting
with the homepage general information and then the [Getting Started](https://urbanmapper.readthedocs.io/en/latest/getting-started/)
section.

Once you have grasped the basics, we recommend exploring the [Interactive Examples](https://urbanmapper.readthedocs.io/en/latest/examples/)
or running yourself the notebooks through the `examples/` directory.

## Licence

`UrbanMapper` is released under the [MIT Licence](./LICENCE).

## Acknowledgments — Community-Led Continuation

We are grateful to **New York University** for supporting the early design and development of `UrbanMapper`, and for
providing an encouraging research environment—especially through the **OSCUR** funding support (https://oscur.org).

**UrbanMapper Community** builds on those initial foundations and continues the work as a community-led effort, with a
focus on transparent collaboration, reproducible workflows, and open participation as well as public roadmap.

This was unfortunately hardly the case through the first `UM` repository, questions were hardly answered, issues left,
and contributions difficult to make through.

<img src="https://vectorseek.com/wp-content/uploads/2023/08/NYU-Logo-Vector.svg-.png" width="200px" alt="New York University logo">
