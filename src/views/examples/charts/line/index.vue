<script lang="tsx">
  import { defineComponent } from 'compatible-vue';

  import { Row, Col } from 'ant-design-vue';
  import { CollapseContainer } from '@/components/container/index';

  import Line1 from './Line1.vue';
  import Line2 from './Line2.vue';
  import Line3 from './Line3.vue';
  import Line4 from './Line4.vue';
  import Line5 from './Line5.vue';
  import Line6 from './Line6.vue';
  import Line7 from './Line7.vue';
  import Line8 from './Line8.vue';
  export default defineComponent({
    setup() {
      return () => {
        return (
          <Row>
            <Col md={24} lg={12} class="p-2">
              <CollapseContainer title="基础" canExpan={false}>
                <Line1 />
              </CollapseContainer>
            </Col>
            <Col md={24} lg={12} class="p-2">
              <CollapseContainer title="区域" canExpan={false}>
                <Line2 />
              </CollapseContainer>
            </Col>
            <Col md={24} lg={12} class="p-2">
              <CollapseContainer title="堆叠区域图" canExpan={false}>
                <Line3 />
              </CollapseContainer>
            </Col>
            <Col md={24} lg={12} class="p-2">
              <CollapseContainer title="多轴面积趋势图" canExpan={false}>
                <Line4 />
              </CollapseContainer>
            </Col>
            <Col md={24} lg={12} class="p-2">
              <CollapseContainer title="未来一周气温变化" canExpan={false}>
                <Line5 />
              </CollapseContainer>
            </Col>
            <Col md={24} lg={12} class="p-2">
              <CollapseContainer title="Setp Line" canExpan={false}>
                <Line6 />
              </CollapseContainer>
            </Col>
            <Col span={24} class="p-2">
              <CollapseContainer title="示例7" canExpan={false}>
                <Line7 height="600px" />
              </CollapseContainer>
            </Col>
            <Col span={24} class="p-2">
              <CollapseContainer title="示例8" canExpan={false}>
                <Line8 height="600px" />
              </CollapseContainer>
            </Col>
          </Row>
        );
      };
    },
  });
</script>
