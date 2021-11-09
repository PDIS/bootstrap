---
layout: docs
title: 側邊欄 Sidebar
description: 放置頁面一邊的具層級性、垂直排列的導覽
group: components
toc: true
---

{{< example >}}

<div class="row">
  <div class="col-md-6">
    <div class="sidebar" id="sidebar">
      <div class="sidebar-item">
        <h2 class="sidebar-header" id="headerone">
          <button class="sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseone" aria-expanded="true" aria-controls="collapseone">
            可展開第一層標題
          </button>
        </h2>
        <div id="collapseone" class="sidebar-collapse collapse" aria-labelledby="headerone" data-bs-parent="#sidebar">
          <div class="sidebar-second-layer" id="sidebarsecondlayer">
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="secondlayerheaderone">
                <button class="sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#secondlayercollapseone" aria-expanded="true" aria-controls="secondlayercollapseone">
                  可展開第二層標題
                </button>
              </h2>
              <div id="secondlayercollapseone" class="sidebar-collapse collapse" aria-labelledby="secondlayerheaderone" data-bs-parent="#sidebarsecondlayer">
              </div>
            </div>
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="secondlayerheadertwo">
                <button class="sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#secondlayercollapsetwo" aria-expanded="true" aria-controls="secondlayercollapsetwo">
                  可展開第二層標題
                </button>
              </h2>
              <div id="secondlayercollapsetwo" class="sidebar-collapse collapse" aria-labelledby="secondlayerheadertwo" data-bs-parent="#sidebarsecondlayer">
                <div class="list-group">
                  <a href="#" class="sidebar-link">
                    可點擊服務連結
                  </a>
                  <a href="#" class="sidebar-link active" aria-current="true">瀏覽中服務連結</a>
                  <a href="#" class="sidebar-link">可點擊服務連結</a>
                  <a href="#" class="sidebar-link">可點擊服務連結</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

{{< /example >}}
