# A simple Jupyter kernel for PostgreSQL

Install the official version with `pip install postgres_kernel`

Install from git repo (experimental) with: `pip install git+https://github.com/mhoangvslev/postgres_kernel/`

To use, run one of:

```bash
jupyter notebook
# In the notebook interface, select PostgreSQL from the 'New' menu
jupyter qtconsole --kernel postgres
jupyter console --kernel postgres
```

## How to use:

There are a couple of specially formatted comments for controlling the connection string and autocommit mode.

```sql
-- connection: postgres://brian:password@localhost:5432/dbname
-- autocommit: true
-- (or false)
```

For details of how this works, see Jupyter's docs on [wrapper kernels](http://jupyter-client.readthedocs.io/en/latest/wrapperkernels.html).
This is heavily based on [takluyver/bash_kernel](https://github.com/takluyver/bash_kernel). Just look at our git log :)

![](images/console.png)

![](images/notebook.png)

## Demonstration:
- [Loiret Photographs Archive](https://github.com/mhoangvslev/PhotographiesArchiveSQL)
- [PostgreSQL Basics](https://github.com/mhoangvslev/JupyterPostgreSQLBasics)

## Progress:
[![Waffle.io - Issues in progress](https://badge.waffle.io/mhoangvslev/postgres_kernel.png?label=in%20progress&title=In%20Progress)](http://waffle.io/mhoangvslev/postgres_kernel)

Related
-------

- Catherine Devlin has an ipython magic that seems very full featured: [catherinedevlin/ipython-sql](https://github.com/catherinedevlin/ipython-sql)

- As noted, this is based on [takluyver/bash_kernel](https://github.com/takluyver/bash_kernel)
