<template>
  <article>
    <section>
      <h1>vue-fraction-grid</h1>

      <container>
        <grid vertical="middle" :rwd="{compact: 'stack'}">
          <grid-item size="1/6" :rwd="{compact: '0/1'}">
            1/6, compact: 0/1
          </grid-item>

          <grid-item size="3/6" :rwd="{compact: '1/1'}">
            3/6, compact: 1/1
          </grid-item>

          <grid-item size="2/6" :rwd="{compact: '1/1'}">
            2/6, compact: 1/1
          </grid-item>
        </grid>
      </container>
    </section>

    <section>
      <h2>Container</h2>

      <container>
        Default
      </container>

      <hr>

      <container width="720px">
        720px
      </container>
    </section>

    <section>
      <h2>Grid</h2>

      <container>
        <grid>
          <grid-item size="1/3">
            1/3
          </grid-item>

          <grid-item size="2/3">
            2/3
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid>
          <grid-item size="2/3">
            <grid>
              <grid-item size="1/2">
                2/3 > 1/2
              </grid-item>

              <grid-item size="1/2">
                2/3 > 1/2
              </grid-item>
            </grid>
          </grid-item>

          <grid-item size="1/3">
            1/3
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid horizontal="left">
          <grid-item size="1/4">
            1/4
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid horizontal="center">
          <grid-item size="1/4">
            1/4
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid horizontal="right">
          <grid-item size="1/4">
            1/4
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid horizontal="around">
          <grid-item size="1/4">
            1/4
          </grid-item>

          <grid-item size="1/4">
            1/4
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid horizontal="between">
          <grid-item size="1/4">
            1/4
          </grid-item>

          <grid-item size="1/4">
            1/4
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid vertical="top">
          <grid-item size="1/2">
            1/2
          </grid-item>

          <grid-item size="1/2">
            1/2
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid vertical="top">
          <grid-item size="1/2" class="lg">
            1/2
          </grid-item>

          <grid-item size="1/2">
            1/2
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid vertical="middle">
          <grid-item size="1/2" class="lg">
            1/2
          </grid-item>

          <grid-item size="1/2">
            1/2
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid vertical="bottom">
          <grid-item size="1/2" class="lg">
            1/2
          </grid-item>

          <grid-item size="1/2">
            1/2
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid flat>
          <grid-item size="3/4">
            3/4
          </grid-item>

          <grid-item size="1/4">
            1/4
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid pair>
          <grid-item size="3/4">
            1/4
          </grid-item>

          <grid-item size="1/4">
            3/4
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid direction="reverse">
          <grid-item size="1/3">
            1/3
          </grid-item>

          <grid-item size="2/3">
            2/3
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid direction="stack">
          <grid-item size="1/3">
            1/3
          </grid-item>

          <grid-item size="2/3">
            2/3
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid direction="stack-reverse">
          <grid-item size="1/3">
            1/3
          </grid-item>

          <grid-item size="2/3">
            2/3
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid horizontal="right" vertical="bottom" direction="reverse" pair>
          <grid-item size="1/6" class="lg">
            1/6
          </grid-item>
          <grid-item size="1/2">
            1/2
          </grid-item>
        </grid>
      </container>
    </section>

    <section>
      <h2>GridItem</h2>

      <container>
        <grid>
          <grid-item size="5/8">
            5/8
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid>
          <grid-item size="1/1">
            1/1
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid>
          <grid-item size="0/1">
            0/1
          </grid-item>

          <grid-item size="1/2">
            0/1 + 1/2
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid>
          <grid-item grow="2">
            2
          </grid-item>

          <grid-item grow="1">
            1
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid>
          <grid-item shrink="1">
            1
          </grid-item>

          <grid-item grow="1">
            1
          </grid-item>
        </grid>
      </container>
    </section>

    <section>
      <h2>Responsive Design (compact: &lt;415px, tablet: &gt;416px, &lt;1100px)</h2>

      <container>
        <grid :rwd="{compact: 'reverse'}">
          <grid-item size="1/4">
            1/4
          </grid-item>

          <grid-item size="3/4">
            3/4
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid direction="stack" :rwd="{compact: 'stack-reverse'}">
          <grid-item size="1/4">
            1/4
          </grid-item>

          <grid-item size="3/4">
            3/4
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid>
          <grid-item size="1/2" :rwd="{compact: '1/1'}">
            1/2, compact: 1/1
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid>
          <grid-item size="1/2" :rwd="{compact: '0/1'}">
            1/2, compact: 0/1
          </grid-item>
        </grid>
      </container>

      <hr>

      <container>
        <grid :rwd="{compact: 'stack'}">
          <grid-item size="1/6" :rwd="{tablet: '0/1', compact: '1/1'}">
            1/6 -> 0/1 -> 1/1
          </grid-item>
          <grid-item size="1/2" :rwd="{tablet: '1/2', compact: '0/1'}">
            1/2 -> 1/2 -> 0/1
          </grid-item>
          <grid-item size="1/3" :rwd="{tablet: '1/2', compact: '1/1'}">
            1/3 -> 1/2 -> 1/1
          </grid-item>
        </grid>
      </container>
    </section>
  </article>
</template>

<style>
.vfg-container {
  text-align: center;
  background-color: #a2d5f2;
}

.vfg-grid {
  text-align: center;
  color: #fafafa;
  background-color: #07689f;
}

.vfg-grid-item {
  text-align: center;
  color: #fafafa;
  background-clip: content-box;
  background-color: #ff7e67;
}

.lg {
  line-height: 3;
}
</style>
