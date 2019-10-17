---
conditions: Default.EE-B2B
title: Page Builder Setup
---

When enabled in the configuration, Page Builder becomes the default content creation tool for CMS Pages, Blocks, and Dynamic Blocks. In addition, the Enable Advanced CMS button offers Page Builder as an option for Categories and Products. You can also choose the default [page layout]({{ site.baseurl }}{% link design/page-layout.md %}) that you want to use for products, categories, and CMS pages. Page Builder is not available for newsletter content that uses the Magento WYSIWYG [editor]({{ site.baseurl }}{% link cms/editor.md %}).

![]({{ site.baseurl }}{% link images/images/config-general-content-management-advanced-content-tools.png %}){: .zoom}
[_Advanced Content Tools_]({{ site.baseurl }}{% link configuration/general/content-management.md %})

## To configure Page Builder

1. On the _Admin_ sidebar, go to **Stores** > _Settings_ > **Configuration**.

1. In the panel on the left under **General**, choose **Content Management**.

1. Under **Advanced Content Tools**, verify that **Enable Page Builder** is set to `Yes`.

1. If you are ready to set up Google Maps, do the following:

   - If necessary, follow the [Get API Key][1]{: target="_blank"} instructions. Then, paste your **Google Maps API Key**.

   - To change the **Google Maps Style**, paste the JSON code that is generated by the [Google Maps APIs Styling Wizard][2].

1. To configure the number of guidelines in the grid, do the following:

   - In the **Default Column Grid Size** field, enter the default number of columns that you want to appear in the grid.

   - In the **Maximum Column Grid Size** field, enter the largest number of columns that you want to be available in the grid.

        ![]({{ site.baseurl }}{% link images/images-ee/config-general-content-management-advanced-content-tools-grid-size.png %}){: .zoom}
        _Column Grid Size_

1. When complete, click <span class="btn">Save Config</span>.

## To configure default layouts

1. On the _Admin_ sidebar, go to **Stores** > _Settings_ > **Configuration**.

1. In the panel on the left under **General**, choose **Web**.

1. Expand the **Default Layouts** section, and do the following:

    ![]({{ site.baseurl }}{% link images/images-ee/config-general-web-default-layouts.png %}){: .zoom}
    [_Default Layouts_]({{ site.baseurl }}{% link configuration/general/web.md %})

    - Choose the **Default Product Layout** that you want to use for product pages.

    - Choose the **Default Category Layout** that you want to use for category pages.

    - Choose the **Default Page Layout** that you want to use for CMS pages.

1. When complete, click <span class="btn">Save Config</span>.

## To disable Page Builder

{: .bs-callout-info}
Disabling Page Builder replaces the Advanced Content Tools with the WYSIWYG [editor]({{ site.baseurl }}{% link cms/editor.md %}), and might cause display errors in the storefront. Content that you created previously with Page Builder might no longer be editable from the Admin.

1. On the _Admin_ sidebar, go to **Stores** > _Settings_ > **Configuration**.

1. In the panel on the left under **General**, choose **Content Management**.

1. Under **Advanced Content Tools**, set **Enable Page Builder** to `No`. 

1. When prompted to confirm, click <span class="btn">Turn Off</span>.

    ![Turn off Page Builder - confirm]({{ site.baseurl }}{% link images/images-ee/config-general-content-management-advanced-content-tools-disable-page-builder-popup.png %}){: .zoom}
    _Are You Sure You Want to Turn Off Page Builder?_

1. When complete, click <span class="btn">Save Config</span>. Then when prompted, [refresh]({{ site.baseurl }}{% link system/cache-management.md %}) any invalid cache.

[1]: https://developers.google.com/maps/documentation/javascript/get-api-key
[2]: https://mapstyle.withgoogle.com/