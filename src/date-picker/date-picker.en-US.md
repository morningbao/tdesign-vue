:: BASE_DOC ::

## API

### DatePicker Props

name | type | default | description | required
-- | -- | -- | -- | --
allowInput | Boolean | false | \- | N
borderless | Boolean | false | \- | N
clearable | Boolean | false | \- | N
defaultTime | String | '00:00:00' | Time selector default value | N
disableDate | Object / Array / Function | - | Typescript：`DisableDate` `type DisableDate = Array<DateValue> \| DisableDateObj \| ((date: DateValue) => boolean)` `interface DisableDateObj { from?: string; to?: string; before?: string; after?: string }`。[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts) | N
disableTime | Function | - | disable time config function。Typescript：`(time: Date) => Partial<{ hour: Array<number>, minute: Array<number>, second: Array<number>, millisecond: Array<number>  }>`。[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts) | N
disabled | Boolean | - | make DatePicker to be disabled | N
enableTimePicker | Boolean | false | \- | N
firstDayOfWeek | Number | 7 | options: 1/2/3/4/5/6/7 | N
format | String | 'YYYY-MM-DD' | \- | N
inputProps | Object | - | Typescript：`InputProps`，[Input API Documents](./input?tab=api)。[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts) | N
label | String / Slot / Function | - | Typescript：`string \| TNode`。[see more ts definition](https://github.com/Tencent/tdesign-vue/blob/develop/src/common.ts) | N
mode | String | date | options: year/quarter/month/week/date | N
placeholder | String / Array | undefined | Typescript：`string` | N
popupProps | Object | - | Typescript：`PopupProps`，[Popup API Documents](./popup?tab=api)。[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts) | N
prefixIcon | Slot / Function | - | Typescript：`TNode`。[see more ts definition](https://github.com/Tencent/tdesign-vue/blob/develop/src/common.ts) | N
presets | Object | - | Typescript：`PresetDate` `interface PresetDate { [name: string]: DateValue \| (() => DateValue) }`。[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts) | N
presetsPlacement | String | bottom | options: left/top/right/bottom | N
readonly | Boolean | false | \- | N
size | String | medium | options: small/medium/large。Typescript：`SizeEnum`。[see more ts definition](https://github.com/Tencent/tdesign-vue/blob/develop/src/common.ts) | N
status | String | default | options: default/success/warning/error | N
suffixIcon | Slot / Function | - | Typescript：`TNode`。[see more ts definition](https://github.com/Tencent/tdesign-vue/blob/develop/src/common.ts) | N
timePickerProps | Object | - | Typescript：`TimePickerProps`，[TimePicker API Documents](./time-picker?tab=api)。[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts) | N
tips | String / Slot / Function | - | Typescript：`string \| TNode`。[see more ts definition](https://github.com/Tencent/tdesign-vue/blob/develop/src/common.ts) | N
value | String / Number / Date | '' | `v-model` is supported。Typescript：`DateValue` `type DateValue = string \| number \| Date`。[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts) | N
defaultValue | String / Number / Date | '' | uncontrolled property。Typescript：`DateValue` `type DateValue = string \| number \| Date`。[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts) | N
valueType | String | - | Typescript：`DatePickerValueType` `type DatePickerValueType = 'time-stamp' \| 'Date' \| 'YYYY' \| 'YYYY-MM' \| 'YYYY-MM-DD' \| 'YYYY-MM-DD HH' \| 'YYYY-MM-DD HH:mm' \| 'YYYY-MM-DD HH:mm:ss' \| 'YYYY-MM-DD HH:mm:ss:SSS'` `type ValueTypeEnum = DatePickerValueType`。[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts) | N
onBlur | Function |  | Typescript：`(context: { value: DateValue; e: FocusEvent }) => void`<br/> | N
onChange | Function |  | Typescript：`(value: DateValue, context: { dayjsValue?: Dayjs, trigger?: DatePickerTriggerSource }) => void`<br/>[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts)。<br/>`import { Dayjs } from 'dayjs'`<br/><br/>`type DatePickerTriggerSource = 'confirm' \| 'pick' \| 'enter' \| 'preset' \| 'clear'`<br/> | N
onConfirm | Function |  | Typescript：`(context: { date: Date, e: MouseEvent }) => void`<br/> | N
onFocus | Function |  | Typescript：`(context: { value: DateValue; e: FocusEvent }) => void`<br/> | N
onPick | Function |  | Typescript：`(value: DateValue) => void`<br/> | N
onPresetClick | Function |  | Typescript：`(context: { preset: PresetDate, e: MouseEvent }) => void`<br/> | N

### DatePicker Events

name | params | description
-- | -- | --
blur | `(context: { value: DateValue; e: FocusEvent })` | \-
change | `(value: DateValue, context: { dayjsValue?: Dayjs, trigger?: DatePickerTriggerSource })` | [see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts)。<br/>`import { Dayjs } from 'dayjs'`<br/><br/>`type DatePickerTriggerSource = 'confirm' \| 'pick' \| 'enter' \| 'preset' \| 'clear'`<br/>
confirm | `(context: { date: Date, e: MouseEvent })` | \-
focus | `(context: { value: DateValue; e: FocusEvent })` | \-
pick | `(value: DateValue)` | \-
preset-click | `(context: { preset: PresetDate, e: MouseEvent })` | \-


### DateRangePicker Props

name | type | default | description | required
-- | -- | -- | -- | --
allowInput | Boolean | false | \- | N
borderless | Boolean | false | \- | N
clearable | Boolean | false | \- | N
defaultTime | Array | ["00:00:00", "23:59:59"] | Time selector default value。Typescript：`string[]` | N
disableDate | Object / Array / Function | - | Typescript：`DisableRangeDate` `type DisableRangeDate = Array<DateValue> \| DisableDateObj \| ((context: { date: DateRangeValue; partial: DateRangePickerPartial }) => boolean)` `interface DisableDateObj { from?: string; to?: string; before?: string; after?: string }` `type DateRangePickerPartial = 'start' \| 'end'`。[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts) | N
disableTime | Function | - | Typescript：`(times: [Date \| null, Date \| null], context: { partial: DateRangePickerPartial }) => Partial<{ hour: Array<number>, minute: Array<number>, second: Array<number> }>`。[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts) | N
disabled | Boolean | - | \- | N
enableTimePicker | Boolean | false | \- | N
firstDayOfWeek | Number | - | options: 1/2/3/4/5/6/7 | N
format | String | - | \- | N
label | String / Slot / Function | - | Typescript：`string \| TNode`。[see more ts definition](https://github.com/Tencent/tdesign-vue/blob/develop/src/common.ts) | N
mode | String | date | options: year/quarter/month/week/date | N
panelPreselection | Boolean | true | \- | N
placeholder | String / Array | - | Typescript：`string \| Array<string>` | N
popupProps | Object | - | Typescript：`PopupProps`，[Popup API Documents](./popup?tab=api)。[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts) | N
prefixIcon | Slot / Function | - | Typescript：`TNode`。[see more ts definition](https://github.com/Tencent/tdesign-vue/blob/develop/src/common.ts) | N
presets | Object | - | Typescript：`PresetRange` `interface PresetRange { [range: string]: DateRange \| (() => DateRange)}` `type DateRange = [DateValue, DateValue]`。[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts) | N
presetsPlacement | String | bottom | options: left/top/right/bottom | N
rangeInputProps | Object | - | Typescript：`RangeInputProps`，[RangeInput API Documents](./range-input?tab=api)。[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts) | N
separator | String | - | \- | N
size | String | medium | options: small/medium/large。Typescript：`SizeEnum`。[see more ts definition](https://github.com/Tencent/tdesign-vue/blob/develop/src/common.ts) | N
status | String | default | options: default/success/warning/error | N
suffixIcon | Slot / Function | - | Typescript：`TNode`。[see more ts definition](https://github.com/Tencent/tdesign-vue/blob/develop/src/common.ts) | N
timePickerProps | Object | - | Typescript：`TimePickerProps`，[TimePicker API Documents](./time-picker?tab=api)。[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts) | N
tips | String / Slot / Function | - | Typescript：`string \| TNode`。[see more ts definition](https://github.com/Tencent/tdesign-vue/blob/develop/src/common.ts) | N
value | Array | [] | `v-model` is supported。Typescript：`DateRangeValue` `type DateRangeValue = Array<DateValue>`。[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts) | N
defaultValue | Array | [] | uncontrolled property。Typescript：`DateRangeValue` `type DateRangeValue = Array<DateValue>`。[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts) | N
valueType | String | - | options: time-stamp/Date/YYYY/YYYY-MM/YYYY-MM-DD/YYYY-MM-DD HH/YYYY-MM-DD HH:mm/YYYY-MM-DD HH:mm:ss/YYYY-MM-DD HH:mm:ss:SSS | N
onBlur | Function |  | Typescript：`(context: { value: DateRangeValue; partial: DateRangePickerPartial; e: FocusEvent }) => void`<br/> | N
onChange | Function |  | Typescript：`(value: DateRangeValue, context: { dayjsValue?: Dayjs[], trigger?: DatePickerTriggerSource }) => void`<br/>[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts)。<br/>`import { Dayjs } from 'dayjs'`<br/> | N
onConfirm | Function |  | Typescript：`(context: { date: Date[], e: MouseEvent, partial: DateRangePickerPartial }) => void`<br/> | N
onFocus | Function |  | Typescript：`(context: { value: DateRangeValue; partial: DateRangePickerPartial; e: FocusEvent }) => void`<br/> | N
onInput | Function |  | Typescript：`(context: { input: string; value: DateRangeValue; partial: DateRangePickerPartial; e: InputEvent }) => void`<br/> | N
onPick | Function |  | Typescript：`(value: DateValue, context: PickContext) => void`<br/>[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts)。<br/>`interface PickContext { e: MouseEvent; partial: DateRangePickerPartial }`<br/> | N
onPresetClick | Function |  | Typescript：`(context: { preset: PresetDate, e: MouseEvent }) => void`<br/> | N

### DateRangePicker Events

name | params | description
-- | -- | --
blur | `(context: { value: DateRangeValue; partial: DateRangePickerPartial; e: FocusEvent })` | \-
change | `(value: DateRangeValue, context: { dayjsValue?: Dayjs[], trigger?: DatePickerTriggerSource })` | [see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts)。<br/>`import { Dayjs } from 'dayjs'`<br/>
confirm | `(context: { date: Date[], e: MouseEvent, partial: DateRangePickerPartial })` | \-
focus | `(context: { value: DateRangeValue; partial: DateRangePickerPartial; e: FocusEvent })` | \-
input | `(context: { input: string; value: DateRangeValue; partial: DateRangePickerPartial; e: InputEvent })` | \-
pick | `(value: DateValue, context: PickContext)` | [see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts)。<br/>`interface PickContext { e: MouseEvent; partial: DateRangePickerPartial }`<br/>
preset-click | `(context: { preset: PresetDate, e: MouseEvent })` | \-


### DatePickerPanel Props

name | type | default | description | required
-- | -- | -- | -- | --
defaultTime | String | '00:00:00' | Time selector default value | N
`Pick<DatePickerProps, 'value' \| 'defaultValue' \| 'disableDate' \| 'disableTime' \| 'enableTimePicker' \| 'firstDayOfWeek' \| 'format' \| 'mode' \| 'presets' \| 'presetsPlacement' \| 'timePickerProps'>` | \- | - | extends `Pick<DatePickerProps, 'value' \| 'defaultValue' \| 'disableDate' \| 'disableTime' \| 'enableTimePicker' \| 'firstDayOfWeek' \| 'format' \| 'mode' \| 'presets' \| 'presetsPlacement' \| 'timePickerProps'>` | N
onCellClick | Function |  | Typescript：`(context: { date: Date, e: MouseEvent }) => void`<br/> | N
onChange | Function |  | Typescript：`(value: DateValue, context: { dayjsValue?: Dayjs, e?: MouseEvent, trigger?: DatePickerTriggerSource }) => void`<br/> | N
onConfirm | Function |  | Typescript：`(context: { date: Date, e: MouseEvent }) => void`<br/> | N
onMonthChange | Function |  | Typescript：`(context: { month: number, date: Date, e?: MouseEvent, trigger: DatePickerMonthChangeTrigger }) => void`<br/>[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts)。<br/>`type DatePickerMonthChangeTrigger = 'month-select' \| 'month-arrow-next' \| 'month-arrow-previous' \| 'today'`<br/> | N
onPanelClick | Function |  | Typescript：`(context: { e: MouseEvent }) => void`<br/> | N
onPresetClick | Function |  | Typescript：`(context: { preset: PresetDate, e: MouseEvent }) => void`<br/> | N
onTimeChange | Function |  | Typescript：`(context: { time: string, date: Date, trigger: DatePickerTimeChangeTrigger, e?: MouseEvent }) => void`<br/>[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts)。<br/>`type DatePickerTimeChangeTrigger = 'time-hour' \| 'time-minute' \| 'time-second'`<br/> | N
onYearChange | Function |  | Typescript：`(context: { year: number, date: Date, trigger: DatePickerYearChangeTrigger, e?: MouseEvent }) => void`<br/>[see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts)。<br/>`type DatePickerYearChangeTrigger = 'year-select' \| 'year-arrow-next' \| 'year-arrow-previous' \| 'today'`<br/> | N

### DatePickerPanel Events

name | params | description
-- | -- | --
cell-click | `(context: { date: Date, e: MouseEvent })` | \-
change | `(value: DateValue, context: { dayjsValue?: Dayjs, e?: MouseEvent, trigger?: DatePickerTriggerSource })` | \-
confirm | `(context: { date: Date, e: MouseEvent })` | \-
month-change | `(context: { month: number, date: Date, e?: MouseEvent, trigger: DatePickerMonthChangeTrigger })` | [see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts)。<br/>`type DatePickerMonthChangeTrigger = 'month-select' \| 'month-arrow-next' \| 'month-arrow-previous' \| 'today'`<br/>
panel-click | `(context: { e: MouseEvent })` | \-
preset-click | `(context: { preset: PresetDate, e: MouseEvent })` | \-
time-change | `(context: { time: string, date: Date, trigger: DatePickerTimeChangeTrigger, e?: MouseEvent })` | [see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts)。<br/>`type DatePickerTimeChangeTrigger = 'time-hour' \| 'time-minute' \| 'time-second'`<br/>
year-change | `(context: { year: number, date: Date, trigger: DatePickerYearChangeTrigger, e?: MouseEvent })` | [see more ts definition](https://github.com/Tencent/tdesign-vue/tree/develop/src/date-picker/type.ts)。<br/>`type DatePickerYearChangeTrigger = 'year-select' \| 'year-arrow-next' \| 'year-arrow-previous' \| 'today'`<br/>


### DateRangePickerPanel Props

name | type | default | description | required
-- | -- | -- | -- | --
defaultTime | Array | ["00:00:00", "23:59:59"] | Time selector default value。Typescript：`string[]` | N
`Pick<DateRangePickerProps, 'value'\| 'defaultValue' \| 'disableDate' \| 'enableTimePicker' \| 'firstDayOfWeek' \| 'format' \| 'mode' \| 'presets' \| 'presetsPlacement' \| 'panelPreselection' \| 'timePickerProps'>` | \- | - | extends `Pick<DateRangePickerProps, 'value'\| 'defaultValue' \| 'disableDate' \| 'enableTimePicker' \| 'firstDayOfWeek' \| 'format' \| 'mode' \| 'presets' \| 'presetsPlacement' \| 'panelPreselection' \| 'timePickerProps'>` | N
onCellClick | Function |  | Typescript：`(context: { date: Date[], partial: DateRangePickerPartial, e: MouseEvent }) => void`<br/> | N
onChange | Function |  | Typescript：`(value: DateRangeValue, context: { dayjsValue?: Dayjs[], partial: DateRangePickerPartial, e?: MouseEvent, trigger?: DatePickerTriggerSource }) => void`<br/> | N
onConfirm | Function |  | Typescript：`(context: { date: Date[], e: MouseEvent }) => void`<br/> | N
onMonthChange | Function |  | Typescript：`(context: { month: number, date: Date[], partial: DateRangePickerPartial, e?: MouseEvent, trigger: DatePickerMonthChangeTrigger }) => void`<br/> | N
onPanelClick | Function |  | Typescript：`(context: { e: MouseEvent }) => void`<br/> | N
onPresetClick | Function |  | Typescript：`(context: { preset: PresetDate, e: MouseEvent }) => void`<br/> | N
onTimeChange | Function |  | Typescript：`(context: { time: string, date: Date[], partial: DateRangePickerPartial, trigger: DatePickerTimeChangeTrigger, e?: MouseEvent }) => void`<br/> | N
onYearChange | Function |  | Typescript：`(context: { year: number, date: Date[], partial: DateRangePickerPartial, trigger: DatePickerYearChangeTrigger, e?: MouseEvent }) => void`<br/> | N

### DateRangePickerPanel Events

name | params | description
-- | -- | --
cell-click | `(context: { date: Date[], partial: DateRangePickerPartial, e: MouseEvent })` | \-
change | `(value: DateRangeValue, context: { dayjsValue?: Dayjs[], partial: DateRangePickerPartial, e?: MouseEvent, trigger?: DatePickerTriggerSource })` | \-
confirm | `(context: { date: Date[], e: MouseEvent })` | \-
month-change | `(context: { month: number, date: Date[], partial: DateRangePickerPartial, e?: MouseEvent, trigger: DatePickerMonthChangeTrigger })` | \-
panel-click | `(context: { e: MouseEvent })` | \-
preset-click | `(context: { preset: PresetDate, e: MouseEvent })` | \-
time-change | `(context: { time: string, date: Date[], partial: DateRangePickerPartial, trigger: DatePickerTimeChangeTrigger, e?: MouseEvent })` | \-
year-change | `(context: { year: number, date: Date[], partial: DateRangePickerPartial, trigger: DatePickerYearChangeTrigger, e?: MouseEvent })` | \-
