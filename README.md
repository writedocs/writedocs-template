# WriteDocs Template

The WriteDocs Template is the foundation for creating and deploying documentation portals using the WriteDocs solution. It comes with everything you need to get started quickly.

## Get Started

To create and deploy your documentation portal using the WriteDocs solution, follow these steps:

1. **Create a Repository from the WriteDocs Template**: Start by creating a new repository using the [WriteDocs Template](https://github.com/writedocs/writedocs-template) on GitHub. Name your repository using the `<yourcompanyname>-docs` pattern.

2. **Connect Your Repository to the WriteDocs App**: Once your repository is set up, add the [WriteDocs App](https://github.com/apps/writedocs-app) to automate the generation and deployment of your documentation. Follow the steps below to connect the WriteDocs App:
3. Access the [WriteDocs App](https://github.com/apps/writedocs-app) page.
4. Click **Install**.
5. Choose **Only select repositories** and select the repository you created in Step 1. That's all you need to do to have your documentation automatically deployed by WriteDocs.

6. **Accessing Your Documentation**: Your documentation will be available at **<yourcompanyname>.docs.WriteDocs.io**. WriteDocs also allows you to customize the documentation domain. For more details, check the [WriteDocs documentation](https://docs.writedocs.io).

## Using the WriteDocs Template

The WriteDocs template includes all the essential components to deploy your documentation portal. Below is an overview of the repository structure and how to use it:

```
|-- config.json
|-- home.html
|-- openapi/
|-- media/
|-- docs/
```

The table below provides instructions on how to use each file and directory available:

| **File/Directory** | **Description**                                                                                                                                                                        |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `config.json`      | All configurations and customizations of your documentation portal are done through this file. Customize appearance, navbar and sidebar structures, colors, and logos here.            |
| `home.html`        | WriteDocs uses the content from this file to generate the homepage of your documentation.                                                                                              |
| `docs/`            | Place all [MDX](https://mdxjs.com/) files in this directory to generate your documentation pages. Organize the files according to the desired structure of your documentation sidebar. |
| `openapi/`         | Upload your OpenAPI files here to generate interactive API pages where customers can test your APIs.                                                                                   |
| `media/`           | Store all images used in your documentation in this directory. You can reference these images when writing your documentation.                                                         |

## Explore Additional Features

For detailed information on how to use all the features offered by WriteDocs, refer to the [WriteDocs documentation](https://docs.writedocs.io).
