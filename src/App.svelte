<script>

	import MouseMove from "./Events/DomEvents.svelte";
	import MouseMoveInline from "./Events/InlineHandlers.svelte";
	import HelloWorld from "./introduction/HelloWorld.svelte";
	import IfCondition from "./logic/IfCondition.svelte";
	import IfElseCondition from "./logic/IfElseCondition.svelte";
	import IfElseIfCondition from "./logic/IfElseIfCondition.svelte";
  	import EachBlocks from "./logic/EachBlocks.svelte";
  	import DynamicAttr from "./introduction/DynamicAttr.svelte";
  	import Styling from "./introduction/Styling.svelte";
  	import HtmlTags from "./introduction/HtmlTags.svelte";
	import Assignments from "./reactivity/Assignments.svelte";
	import Declarations from "./reactivity/Declarations.svelte";
	import Statements from "./reactivity/Statements.svelte";
	import UpdatingArrAndObj from "./reactivity/UpdatingArrAndObj.svelte";
	import DeclareProps from "./props/DeclareProps.svelte";
	import DefaultValue from "./props/DefaultValue.svelte";
	import SpreadProps from "./props/SpreadProps.svelte";
	import KeyedEachBlock from "./logic/KeyedEachBlock.svelte";
	import AwaitBlocks from "./logic/AwaitBlocks.svelte";
	import DomEvents from "./Events/DomEvents.svelte";
	import InlineHandlers from "./Events/InlineHandlers.svelte";
	import EventModifiers from "./Events/EventModifiers.svelte";
	import ComponentEvents from "./Events/ComponentEvents.svelte";
	import EventForwarding from "./Events/EventForwarding.svelte";
	import DomEventForwarding from "./Events/DomEventForwarding.svelte";
	import TextInputs from "./bindings/TextInputs.svelte";
	import NumericInputs from "./bindings/NumericInputs.svelte";
	import CheckboxInputs from "./bindings/CheckboxInputs.svelte";
	import GroupInputs from "./bindings/GroupInputs.svelte";
	import TextareaInputs from "./bindings/TextareaInputs.svelte";
	
</script>

<HelloWorld />
<DynamicAttr />
<Styling />
<HtmlTags />
<Assignments />
<hr>
<Declarations />
<hr>
<Statements />
<hr>
<UpdatingArrAndObj />
<hr>
<DeclareProps answer={42}/>
<hr>
<DefaultValue />
<DefaultValue answer={1363}/>
<hr>
<SpreadProps />
<hr>
<IfCondition />
<IfElseCondition />
<IfElseIfCondition />
<hr>
<EachBlocks />
<hr>
<KeyedEachBlock />
<hr>
<AwaitBlocks />
<hr>
<DomEvents />
<hr>
<InlineHandlers />
<hr>
<EventModifiers />
<hr>
<ComponentEvents />
<hr>
<EventForwarding />
<hr>
<DomEventForwarding />
<hr>
<TextInputs />
<hr>
<NumericInputs />
<hr>
<CheckboxInputs />
<hr>
<GroupInputs />
<hr>
<TextareaInputs />